# 1) Quantas vezes Natalie Portman foi indicada ao Oscas?
Resposta: 3 vezes

 `SELECT COUNT(*) FROM indicados WHERE "Name" Like "%Natalie Portman%";`
# 2) Quantos Oscars Natalie Portman ganhou?

Resposta: Ela ganhou 1 Oscar.

Q:

`SELECT * FROM indicados_ao_oscar WHERE nome_do_indicado like "%Natalie Portman%" AND vencedor = "true";`
