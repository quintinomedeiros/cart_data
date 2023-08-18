# Dados do Cartola FC



# *CARTOLA_DATA*
Compreende um  conjunto de DataSets com o dados analisados e corrigidos dos jogadores participantes do CartolaFC.
Os arquivos possuem a seguinte padronização no nome: # *cart_data_{ano}.csv*, são do tipo .csv e estão divididos por temporada e possuem os seguintes campos:


# *Campos de identificação* (inteiro  ou texto)

*temporada_id:* identificador da temporada, formada pelo ano formado por 4 digitos

*rodada_id:* identificador da rodada, formado por identificador de até 2 dígitos

*clube_id:* identificador do clube do atleta, formado por indentificador de 3 dígitos

*atleta_id:* identificador do atleta, formado por cinco a seis dígitos

# *Campos de pontuação* (flutuante ou inteiro)

*atleta_pontos:* pontuação ponderada dos atletas, formada pelo somatório da multiplicação por atleta em cada rodada dos scouts multiplicados pelos respectivos pesos na rodada

*atleta_media:* pontuação média dos atletas nas rodadas anteriores

*atleta_preco:* valor em cartoletas (moeda do fantasy game) para escalação do atleta

*atleta_preco_variacao:* aumento do decremento do valor do atleta em relação à rodada anterior

*DS:* frequência do scout de desarme para o atleta na rodada (antigo roubada de bola RB)

*FC:* frequência do scout de falta cometida para o atleta na rodada

*GC:* frequência do scout de gol contra para o atleta na rodada

*CA:* frequência do scout de cartão amarelo para o atleta na rodada

*CV:* frequência do scout de cartão vermelho para o atleta na rodada

*SG:* frequência do scout de sem gol para o atleta na rodada

*DP:* frequência do scout de defesa de panaltin para o atleta na rodada

*GS:* frequência do scout de gol sofrido para o atleta na rodada

*FS:* frequência do scout de falata sofrida para o atleta na rodada

*A:* frequência do scout de assistência para o atleta na rodada

*FT:* frequência do scout de finalização na trave para o atleta na rodada

*FD:* frequência do scout de finalização defendida para o atleta na rodada

*FF:* frequência do scout de finalização para fora para o atleta na rodada

*G:* frequência do scout de gol para o atleta na rodada

*I:* frequência do scout de impedimento para o atleta na rodada

*PP:* frequência do scout de pênalti perdido para o atleta na rodada

*PS:* frequência do scout de pênalti sofrido para o atleta na rodada

*DE:* frequência do scout de defesa para o atleta na rodada

*V:* frequência do scout de vitória para o atleta na rodada


# *Dados do clube* (inteiro e booleano)

*clube_gol_pro:* gol(s) marcado(s) pelo time do atleta na rodada

*clube_col_con:* gol(s) sofrido(s) pelo time do atleta na rodada

*clube_part_res:* total de pontos conseguidos pelo time do atleta na rodada (vitória = 3; empate = 1; derrota = 0)

*clube_mand:* indicação se o clube do atleta foi mandante (1) ou visitante (0) na rodada

#*CARTOLA_INFO*
Compreende um  conjunto de DataSets com as informações referentes aos clubes, posições dos atletas e status dos atletas na rodada, sendo formado pelos seguintes arquivos:
# *cartola_clubes.csv*
# *cartola_posicoes.csv*
# *cartola_status.csv*
