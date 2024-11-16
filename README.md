# 1) Quantas vezes Natalie Portman foi indicada ao Oscas?
Resposta: 3 vezes

 `SELECT COUNT(*) FROM indicados WHERE "Name" Like "%Natalie Portman%";`
# 2) Quantos Oscars Natalie Portman ganhou?

Resposta: Ela ganhou 1 Oscar.

Q:

`SELECT * FROM indicados_ao_oscar WHERE nome_do_indicado like "%Natalie Portman%" AND vencedor = "true";`
# 3) Amy Adams já ganhou algum Oscar?

Resposta: Não Amy Adams nunca ganhou o Oscar.

Q:

`SELECT * FROM indicados_ao_oscar WHERE nome_do_indicado like "%Amy Adams%";`
# 4) A série de filmes Toy Story ganhou um Oscar em quais anos?

Resposta: Toy Story ganhou o Oscar em 2011 e 2020.

Q:

`SELECT * FROM indicados_ao_oscar WHERE nome_do_filme like "%Toy Story%" AND vencedor = "true";`
# 5) A partir de que ano a categoria "Actress" deixa de existir?

Resposta: Ela deixa de existir a partir de 1977.

Q:

`SELECT * FROM indicados_ao_oscar WHERE categoria = "ACTRESS" ORDER BY ano_cerimonia DESC;`


