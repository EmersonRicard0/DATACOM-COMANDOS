# DATACOM-COMANDOS
Uma ajuda com comandos para auxiliar na verificação e configuração de olt e sw  DATACOM



###DATACOM##COMANDOS###
::::MODO GLOBAL  VERICICAÇÕES:::
show running-config ("verifica todas as configurações feitas")

show running-config dot1q (" é possivel verificar por blocos , por exemplo de vlans:"dot1q") 

show environment  ("verifica a parte de temperatura do equipamento")

show firmware ("status de atualização, progresso de intalação e versão ativa de firmware")

show inventory ("verifica informações sobre o equipamento,como: serial, tipos de portas")

show platform (" verifica modelo do equipamento, versão de firmware , tipo de fontes")

show tech-support ("trás todos os show existentes em um só comando")

show alarm ("Verifica alarmes no equipamento")

:::VERIFICAÇÃO INTERFACE ETHERNET:::
show interface gigabit-ethernet 1/1/1 ("O comando trás status da porta ")

show interface link ("vai trazer todos as portas na descrição , status ")

show interface transceivers ("Trás status dos modelos sfp e gpon")

:::VERIFICAÇÃO DE VLANS:::
show vlan brief ("Resumo das vlans")

show vlan membership brief ("Verifica a quais membros a vlan está associada")

show running-config dot1q | tab (" verificação de vlans ,| tab serve para transforma a descrição em tabela")

:::VERIFICAÇÃO DE GPON:::

show interface gpon 1/1/1 ("Vai trazer informações da interface gpon 1/1/1 ")

show interface gpon 1/1/1 onu ("vai trazer informações de todas as onus autorizadas na interface gpon")

show interface gpon 1/1/1 onu 0 ("vai trazer informações sobre a onu dessa interface")

show interface gpon 1/1/1 onu 0 ethernet ("Verifica a porta ethernet da onu, se esta up ou down")

show interface gpon 1/1/1 discovered-onus("Verifica se há onus para autorizar ")

show running-config profile gpon bandwidth-profile("verifica todos os profiles para determinados serviços pppoe,dhcp,gerencia entre outros")

show running-config profile gpon line-profile(" é oque esta entregando ao cliente")

