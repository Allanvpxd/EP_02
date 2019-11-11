# EP_02
# Cadastramento de usuários com Rabbitmq(pika),Python,Mongodb via docker.
########################################################################################################
# AUTOR: ALLAN VINICIUS PINTO                                                                          #
#                                                                                                      #
# PROCESSO: IREMOS REALIZAR A INSTALACAO DO PYMONGO, RABBITMQ, PIKA, REQUESTS VIA IMAGEM DOCKER        #
#           MONGO FICA INSTANCIADO LOCALMENTE                                                          #
#           RABBITMQ FICA INSTANCIADO VIA DOCKER (127.0.0.1:15672)                                     #
#           NOSSO PROCESSO IRA ENVIAR MENSAGENS VIA PRODUTO PARA OS CONSUMIDORES,                      #
#           ONDE IREMOS GRAVAR OS DADOS NO MONGODB EM 3 BASES:                                         #
#           USUARIOS: ONDE IREMOS TER OS REGISTROS DOS USUARIOS                                        #
#           EVENTOS: ONDE IREMOS TER OS REGISTROS DE TODOS OS PROCESSOS REALIZADOS NA BASE DE USUARIOS #
#           VOLUME: ONDE IREMOS TER A QUANTIDADE DE USUARIOS CADASTRADOS                               #
#                                                                                                      #
########################################################################################################
#                                                                                                      #
# REQUISITOS:                                                                                          #
# -> DOCKER INSTALADO                                                                                  #
# -> DOCKER-COMPOSE INSTALADO                                                                          #
#                                                                                                      #
# EXECUCAO                                                                                             #
# -> LOGAR NO DOCKER                                                                                   #
#  -> DOCKER LOGIN                                                                                     #
#                                                                                                      #
# -> RODAR O COMANDO DOCKER-COMPOSE                                                                    #
#  -> DOCKER-COMPOSE UP --BUILD                                                                        #
#                                                                                                      #
# -> ABRIR EM ABAS DIFERENTES DO CONSOLE                                                               #
#  -> ABRIR A PASTA CONSUMER_EVENT                                                                     #
#  -> EXECUTAR O COMANDO: PYTHON3 CONSUMER_EVENT.PY                                                    #
#                                                                                                      #
#  -> ABRIR A PASTA CONSUMER_USER                                                                      #
#  -> EXECUTAR O COMANDO: PYTHON3 CONSUMER_USER.PY                                                     #
#                                                                                                      #
#  -> ABRIR A PASTA CONSUMER_VOLUME                                                                    #
#  -> EXECUTAR O COMANDO: PYTHON3 CONSUMER_VOLUME.PY                                                   #
#                                                                                                      #
#  -> ABRIR A PASTA PRODUCTOR                                                                          #
#  -> EXECUTAR O COMANDO: PYTHON3 PRODUCTOR.PY                                                         #
#  -> SELECIONAR A OPÇÃO QUE DESEJA REALIZAR (1=INSERT,2=DELETE,3=UPDATE)                              #
#  -> PASSAR AS INFORMACOES SOLICITADAS                                                                #
#                                                                                                      #
########################################################################################################
