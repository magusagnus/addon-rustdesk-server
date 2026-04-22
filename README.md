# Home Assistant Add-on: RustDesk Server

[![Relançamentos do GitHub][releases-shield]][releases]
[![Licença][license-shield]][license]
![Arquitetura Suportada][amd64-shield]

Este add-on permite que você execute seu próprio servidor de sinalização e revezamento (hbbs/hbbr) para o **RustDesk** diretamente no seu Home Assistant.

[RustDesk](https://rustdesk.com/) é uma alternativa de desktop remoto de código aberto, que permite que você mantenha total controle sobre seus dados e segurança, sem depender de servidores de terceiros.

## 🚀 Instalação Rápida

Para adicionar este repositório ao seu Home Assistant, clique no botão abaixo:

[![Adicionar repositório ao Home Assistant][add-repo-badge]](https://my.home-assistant.io/redirect/supervisor_add_repo/?repository_url=https%3A%2F%2Fgithub.com%2Fmagusagnus%2Faddon-rustdesk-server)

Ou adicione manualmente a URL:
`https://github.com/magusagnus/addon-rustdesk-server`

---

## 🔥 Sobre este Fork
Este projeto é um **fork** baseado no excelente trabalho original. Foram realizadas melhorias técnicas para garantir a estabilidade no Supervisor atual, incluindo:

- 🛠 **Correção de Build**: Ajuste no gerenciador de pacotes para evitar falhas de versão do `unzip`.
- 🏗 **Otimização amd64**: Configurado especificamente para arquiteturas 64 bits.
- ⚡ **Atualização**: Baseado na versão estável 1.1.15 do RustDesk Server.

### 🙏 Agradecimentos
Um agradecimento especial ao autor original do repositório (Frosh) por fornecer a base sólida que permitiu a criação deste add-on. Projetos de código aberto crescem através da colaboração e do compartilhamento!

---

## ⚙️ Configuração do Cliente
Após instalar o add-on, você deve configurar o seu cliente RustDesk (PC ou Celular):

1. Vá em **Configurações > Rede**.
2. No campo **Servidor de ID**, coloque o IP do seu Home Assistant.
3. Se você definiu uma chave nas opções do add-on, coloque-a no campo **Chave**.
4. Verifique se o status na parte inferior do cliente mudou para **"Pronto"**.

## 🛡️ Portas Utilizadas
Certifique-se de que as seguintes portas estejam acessíveis (e redirecionadas no seu roteador se precisar de acesso externo):
- `21115` (TCP)
- `21116` (TCP/UDP)
- `21117` (TCP)
- `21118` (TCP)
- `21119` (TCP)

---
**Mantido por:** [magusagnus](https://github.com/magusagnus)

[releases-shield]: https://img.shields.io/github/v/release/magusagnus/addon-rustdesk-server?style=for-the-badge
[releases]: https://github.com/magusagnus/addon-rustdesk-server/releases/tag/v.1.1.15-magus
[license-shield]: https://img.shields.io/github/license/magusagnus/addon-rustdesk-server?style=for-the-badge
[license]: LICENSE
[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg?style=for-the-badge
[add-repo-badge]: https://my.home-assistant.io/badges/supervisor_add_repo.svg
