# harpia-seed-data

JSONs estaticos (Camara dos Deputados + TSE) consumidos pelo db/seeds.rb dos alunos.


Este repositório só tem os dados. O template do `db/seeds.rb` que os alunos
colam no projeto deles está em `db/seeds.rb` na branch `main` de
[harpia_db](https://github.com/gabsgarcia/harpia_db) — ele já baixa esses
JSONs pelo BASE_URL acima e popula as 4 tabelas centrais (Partido, Politico,
Votacao, Voto). As outras 4 (Despesa, Proposicao, Candidato2026,
MotivoCassacao) vêm como bloco bônus comentado no mesmo arquivo, pra quem
terminar o MVP cedo. Os models e migrations são conteúdo de aula — ver
`modelo-referencia` no harpia_db para o gabarito.
Gerados pela rake task em outro repo

## Fotos dos candidatos 2026

O TSE só publica as fotos dos candidatos dentro de ZIPs por UF
(`cdn.tse.jus.br/.../eleicoes2026/fotos/foto_cand2026_{UF}_div.zip`), sem URL
individual. Por isso elas estão hospedadas aqui em `fotos/candidatos_2026/`, e
cada registro de `candidatos_2026.json` tem `url_foto` apontando para o arquivo
via raw.githubusercontent (mesmo nome de campo de `deputados.json`).
