# monitoramento_indicadores_contratuais
Este projeto tem como objetivo identificar comportamentos anômalos em contratos de atendimento telefônico, com base em padrões históricos de chamadas. A análise considera frequência, horários e ausência de chamadas recentes, gerando alertas automáticos por e-mail para facilitar a tomada de decisão e o monitoramento proativo.

# 📞 Detecção de Anomalias em Chamadas com Python

Este projeto tem como objetivo identificar **comportamentos anômalos em contratos de atendimento telefônico**, com base em padrões históricos de chamadas. A análise considera frequência, horários e ausência de chamadas recentes, gerando alertas automáticos por e-mail para facilitar a tomada de decisão e o monitoramento proativo.

---

## 🔍 Funcionalidades

- Leitura de dados históricos de chamadas a partir de uma planilha Excel.
- Identificação de contratos que costumam receber chamadas em horários específicos, mas que **não receberam chamadas recentemente**.
- Aplicação de critérios como:
  - Mais de 5 dias com chamadas no mesmo horário nos últimos 90 dias.
  - Ausência de chamadas nas últimas 2 horas.
  - Última ligação há no máximo 5 dias.
  - Frequência de chamadas superior a 30% nos últimos 30 dias.
- Cálculo de indicadores como:
  - **NS (%)** – Nível de Serviço.
  - **Taxa de Abandono (%)** – Proporção de chamadas não atendidas.
- Envio automático de e-mail com os contratos identificados como anômalos ou mensagem explicativa caso não haja alertas.

---

## 🛠️ Tecnologias Utilizadas

- **Python 3**
- **Pandas** – Manipulação de dados.
- **datetime** – Cálculos de tempo e datas.
- **smtplib / email.mime** – Envio de e-mails automatizados.
- **openpyxl** – Leitura de arquivos Excel.

---

## 🚀 Como Usar

1. Substitua os campos no script:
   - `SEU_EMAIL_AQUI`, `SUA_SENHA_AQUI`, `SMTP_SERVER_AQUI`, etc.
   - Nome da planilha Excel e nomes das colunas conforme seu dataset.

2. Execute o script:
   ```bash
   python detectar_anomalias_chamadas.py

   O sistema analisará os dados e enviará um e-mail com os contratos que apresentaram comportamento fora do padrão.


💡 Motivação
Este projeto foi desenvolvido para automatizar a detecção de possíveis falhas ou interrupções no fluxo de atendimento, permitindo ações corretivas rápidas e baseadas em dados. Ideal para equipes de suporte, operações ou gestão de contratos.

📫 Contato
Rafael Rocha Gorgonio
LinkedIn: www.linkedin.com/in/rafael-gorgonio | Email: rafaelrgorgonio@gmail.com

Sinta-se à vontade para contribuir ou sugerir melhorias!
