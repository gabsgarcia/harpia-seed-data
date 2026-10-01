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
