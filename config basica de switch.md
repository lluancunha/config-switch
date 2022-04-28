!acessar o modo EXEC privilegiado
    enable

!comfigurar a data e hora (mes em ingles)
    clock set 19:30:00 28 April 2022

!modo de configuração global (abreviado = conf t)
    configure terminal 

!configuração do hostname (nome do equipamento)
    hostname sw-01

!habilitar criptografia de senha 
    service password-encryption

!habilitar a marcaçao de data e hora no log 
    service timestamps log datetime msec

!desativar a resoluçao de nome
    no ip domain-lookup

!configuração da mensagem do dia 
    banner motd #AVISO acesso autorizado somente a funcionarios#

!habilitar a senha do modo enable
    enable secret 123@senac

!criar usuarios de administraçao do switch
    username senac secret 123@senac

!acesaar a linha de console 
    line console 0 

!habilitar login local
    login local

!habilitar o sincronismo dos logs 
    logging synchronous

!habilitar o tempo de inatividade 
    exec-timeout 5 30 

!sair de todos os modos (atalho = ctrl z)
    end

!salvar as config do switch
    copy running-config startup-config

!verificar as configs do switch 
    show running-config



