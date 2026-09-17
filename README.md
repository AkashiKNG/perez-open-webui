# Open WebUI para o Perez OS

Interface de chat ([Open WebUI](https://github.com/open-webui/open-webui)) pronta para importar no Perez OS, com:

- **Modelos grátis do gpt4free**: um gpt4free sem interface roda junto, só na rede interna do app, sem os
  provedores que exigem login.
- **NVIDIA NIM**: conexão direta com `https://integrate.api.nvidia.com/v1` usando `NVIDIA_NIM_API_KEY`.

## Uso

1. Importe `https://github.com/AkashiKNG/perez-open-webui` no painel.
2. No card, preencha `NVIDIA_NIM_API_KEY` (ou deixe vazio para usar só o gpt4free).
3. Abra a UI e clique em **Cadastre-se**: a primeira conta vira a administradora. Os modelos aparecem no
   seletor do chat.
4. Criada a conta, coloque `OPEN_WEBUI_ENABLE_SIGNUP=false` no card e atualize, para fechar o cadastro.

As conexões e o cadastro vêm sempre das variáveis (`ENABLE_PERSISTENT_CONFIG=false`): mudar no card e
atualizar o repo basta, sem mexer em **Configurações → Conexões** dentro da interface.
