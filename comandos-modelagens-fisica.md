# Comandos SQL para modelagem física

## Criar banco de dados
CREATE DATABASE vendas_Misael CHARACTER SET utf8mb4;

## Entrar no banco de dados criado
USE DATABASE vendas_misael;

## Criar tabela fabricantes
CREATE TABLE fabricantes(
    id INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(45) NOT NULL
);

## Criar tabela produto
CREATE TABLE produtos(
    id INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
    nome VARCHAR(45) NOT NULL
    preco DECIMAL(8,2) NOT NULL,
    quantidade SMALLINT NULL,
    descricao TEXT(1000) NOT NULL,
    fabricante_id INT NOT NULL,
);

## Alterando a tabela para criar um relacionamento por meio da chave estrageira
ALTER TABLE produtos
    ADD CONSTRAINT fk_produtos_fabricantes
    FOREIGN KEY(fabricante_id) REFERENCES fabricantes(id);

