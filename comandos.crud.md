# Comandos CRUD SQL

## Resumo da sigla
- C -> CREATE (INSERT, inserir dados)
- R -> READ (SELECT, leitura dados)
- U -> UPDATE (UPDATE, atualizar dados)
- D -> DELETE (INSERT, escluir dados)

## INSERT
INSERT INTO fabricantes(nome) VALUES('Asus');
INSERT INTO fabricantes(nome) VALUES('Dell');
INSERT INTO fabricantes(nome) VALUES('Apple');
INSERT INTO fabricantes(nome) VALUES('LG');

INSERT INTO fabricantes(nome)
VALUES('Samsung),('Microsoft'),('Brastemp');

### Produtos
INSERT INTO produtos(nome, preco, quantidade, descicao, fabricantes_id)
VALUES('TV Led', 2000, 5, 'TV de ultima geração', 5);

INSERT INTO produtos(nome, preco, quantidade, descicao, fabricantes_id)
VALUES('iPhone XYZ', 5500.79, 8, 'Smartphone caro pra caramba', 3);

INSERT INTO produtos(nome, preco, quantidade, descricao, fabricante_id) VALUES
(
    'Geladeira',
    1500,
    10,
    'Refrigerador Frost-free com acesso à Internet das Coisas e bla bla bla',
    7 -- Brastemp
),
(
    'iPad Mini',
    5000,
    8,
    'Tablet Apple com tela retina display de 4k, memória interna de 64GB, acesso ao iCloud.',
    3 -- Apple
),
(
    'Xbox',
    2500,
    6,
    'Console de última geração com acesso aos melhores jogos e bla bla',
    6 -- Microsoft
),
(
    'Ultrabook',
    4500.68,
    12,
    'Equipamento com processador AMD Ryzen5, 12GB de RAM, placa de vídeo RTX',
    1 -- Asus
),
(
    'Headset',
    120,
    9,
    'Fone de ouvido USB com alta qualidade',
    6 -- Microsoft
),
(
    'Tablet Android',
    4999,
    3,
    'Tablet com a versão 12 do sistema operacional da Google, possui tela de 10 polegadas e armazenamento de 64GB.',
    5 -- Samsung
);