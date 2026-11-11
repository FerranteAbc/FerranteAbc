# Pedro Henrique Ferrante Prado

Analista de Sistemas em formação em Defesa Cibernética na FIAP, com foco em **blue team**: detecção, análise de logs e de tráfego, forense e resposta a incidentes, com base ofensiva em pentest.

Busco oportunidades em cybersecurity e segurança da informação, com foco em blue team.

- Portfólio: https://ferranteabc.github.io/meu-portfolio/
- LinkedIn: https://www.linkedin.com/in/pedro-henrique-ferrante-prado-128123230/
- Contato e currículo em PDF: https://ferranteabc.github.io/meu-portfolio/#contato

## O que está documentado aqui

Todos os testes foram feitos em laboratório próprio, em ambiente de homologação da faculdade ou em plataformas de CTF. Cada repositório tem comandos, evidências e write-ups.

| Repositório | O que é |
| :--- | :--- |
| [Cyber-Defense-Project](https://github.com/FerranteAbc/Cyber-Defense-Project) | Avaliação de segurança de uma aplicação web em homologação (FIAP Challenge 2026): 4 achados classificados em CVSS v3.1, plano de correção e critério de reteste. |
| [FIAP-CTF-Write-ups-Solu-es-de-Ciberseguran-a](https://github.com/FerranteAbc/FIAP-CTF-Write-ups-Solu-es-de-Ciberseguran-a) | CTF Trilha 1 (9 desafios de OSINT, threat intelligence e forense de redes, com mapeamento para MITRE ATT&CK), Wargames 2TDCOR (20 desafios de pentest, protocolos e forense) e laboratório com Kali Linux e Metasploitable 2. |
| [Global-Solution-CTF-Wargames](https://github.com/FerranteAbc/Global-Solution-CTF-Wargames) | CTF Global Solution FIAP: 15 desafios resolvidos, com um write-up por desafio (forense de rede, firmware, análise de scripts, criptografia e esteganografia). |
| [Firmware-Reversing-IoT-Security-Forensics](https://github.com/FerranteAbc/Firmware-Reversing-IoT-Security-Forensics) | Segurança IoT e engenharia reversa de firmware com OWASP IoTGoat: 8 desafios de auditoria embarcada e forense digital. |
| [meu-portfolio](https://github.com/FerranteAbc/meu-portfolio) | Código do meu portfólio: site estático, sem rastreadores, com política de segurança de conteúdo (CSP) restritiva. |

## Foco em blue team

- **Detecção:** triagem de logs de autenticação, de acesso web e de eventos do Windows (`.evtx`) para achar força bruta, varreduras automatizadas e movimentação lateral. Snort e Suricata em laboratório.
- **Análise e forense:** inspeção de pacotes com Wireshark e tshark (exfiltração por DNS e HTTP POST, C2, Evil Twin em 802.11), perícia de e-mail (SPF, DKIM e DMARC) e de arquivos.
- **Threat intelligence:** IoCs até as TTPs (Pirâmide da Dor), mapeamento para MITRE ATT&CK e leitura de intrusões pela Cyber Kill Chain.
- **Contenção e hardening:** cada achado com prioridade, correção e critério de reteste.

Exemplo de triagem, tirado dos meus write-ups (IPs com mais falhas de login SSH):

```bash
grep "Failed password" /var/log/auth.log \
  | awk '{print $(NF-3)}' \
  | sort | uniq -c | sort -nr
```

## Ferramentas

Wireshark, tshark, tcpdump, Snort, Suricata, Nmap, Gobuster, Dirsearch, Nikto, Metasploit, Hydra, John the Ripper, binwalk, CyberChef, ExifTool, Python, Bash, PowerShell e Git.
