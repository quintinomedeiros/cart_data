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

# *CARTOLA_INFO*

Compreende um conjunto de DataSets com as informações referentes aos clubes, posições dos atletas e status dos atletas na rodada, sendo formado pelos seguintes arquivos:

*cartola_clubes.csv:* clube_id; clube_nome; clube_abr

*cartola_posicoes.csv:* posicao_id; posicao_nome; posicao_abr

*cartola_status.csv:* status_id; status_nome

# *CARTOLA_PARTIDAS*

Compreende um conjunto de DataSets com as informações referentes às partidas realizadas pelos clubes durante as temporadas de 2014 a 2022, sendo formado por arquivos que possuem o seguinte padrão:

*partidas_cartola_{ano}.csv:* rodada_id; clube_mand; clube_vis; clube_mand_gol; clube_vis_gol; clube_mand_ca; clube_vis_ca; clube_mand_cv; clube_vis_cv

# *CARTOLA_ROD_ATUAL*

Compreende um conjunto de DataSets com as informações referentes à situação dos atletas na rodada atual. É formado por um arquivo resumido com as informações e os scouts principais dos atletas na rodada atual e outro com essas informações mais métricas fornecidas pelo CartolaFC através do Gato-Mestre:

*cartola_atletas.csv:* atleta_id; clube_id; posicao_id; status_id; atleta_apelido; rodada_id; atleta_jogos; atleta_preco; atleta_variacao; atleta_min_val; media_num; atleta_pontos

*cartola_atletas_final.csv:* atleta_id; clube_id; posicao_id; status_id; atleta_apelido; rodada_id; atleta_jogos; atleta_preco; atleta_variacao; atleta_min_val; media_num; atleta_pontos; CA; DS; FC; FS; FT; SG; FD; FF; G; I; PS; A; CV; PC; V; DE; GS; PP; DP; GC; media_pontos_mandante; media_pontos_visitante; media_minutos_jogados; minutos_jogados; gm_media_CA; gm_media_DS; gm_media_FC; gm_media_FS; gm_media_FT; gm_media_SG; gm_media_FD; gm_media_FF; gm_media_G; gm_media_I; gm_media_PS; gm_media_A; gm_media_CV; gm_media_PC; gm_media_DE; gm_media_GS; gm_media_PP; gm_media_DP; gm_media_GC; gm_man_CA; gm_man_DS; gm_man_FC; gm_man_FS; gm_man_FT; gm_man_SG; gm_man_FD; gm_man_FF; gm_man_G; gm_man_I; gm_man_PS; gm_man_A; gm_man_CV; gm_man_PC; gm_man_DE; gm_man_GS;gm_man_PP;gm_man_DP;gm_man_GC; gm_vis_CA; gm_vis_DS; gm_vis_FC; gm_vis_FS; gm_vis_FT; gm_vis_SG; gm_vis_FD; gm_vis_FF; gm_vis_G; gm_vis_I; gm_vis_PS; gm_vis_A; gm_vis_CV; gm_vis_PC; gm_vis_DE; gm_vis_GS; gm_vis_PP; gm_vis_DP; gm_vis_GC
