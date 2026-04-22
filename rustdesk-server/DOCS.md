# Home Assistant Add-on: RustDesk-server

## Sobre / About

Este add-on permite que você auto-hospede seu próprio servidor [RustDesk][rustdesk] no seu Home Assistant (otimizado para arquitetura **amd64**).

Se você utiliza o RustDesk, é altamente recomendável ter seu próprio [servidor RustDesk][serveur_rustdesk]. Os servidores públicos do RustDesk são destinados a fins de teste e pesquisa e não estão equipados para lidar com grandes volumes de tráfego. Ter seu próprio servidor garante velocidade máxima, estabilidade e total controle sobre sua privacidade.

##### _This add-on allows you to self-host your own [RustDesk][rustdesk] server on your Home Assistant (optimized for **amd64** architecture). Using your own server ensures faster connection times, better reliability, and full control over your data and relay traffic._

---

## Instalação / Installation

1. Adicione este repositório à sua Loja de Add-ons do Home Assistant:
   `https://github.com/magusagnus/addon-rustdesk-server`

[![Adicionar repositório ao Home Assistant][add-repo-shield]][add-repo]

2. Procure por **RustDesk Server** na loja e clique em instalar.

---

## Configuração / Configuration

Exemplo de configuração básica / Example app configuration:

```yaml
private_key: "pmuglkSV..."
public_key: "bhy1kWGC..."
relay: "seu-dominio.duckdns.org"
```


**Nota:** Este é apenas um exemplo. Gere suas próprias chaves para maior segurança! / This is just an example, create your own keys!
Opções / Options:

+ private_key: Parte privada do par de chaves. Força o uso de uma chave específica.

+ public_key: Parte pública do par de chaves. Necessária para que os clientes se conectem com segurança.

+ relay: Endereço IP ou DNS do servidor executando o hbbr (geralmente o IP do seu HA).

---

### Fork & Créditos / Credits

Este repositório é um fork técnico do projeto original de Frosh/casse-boubou.

As modificações realizadas por magusagnus visam:

1. Corrigir falhas de build no Supervisor (conflitos de versão do unzip no Alpine Linux).

2. Garantir compatibilidade nativa com arquiteturas amd64/x86_64.

3. Manter o servidor atualizado com as últimas releases estáveis do RustDesk.

---

### Agradecimentos / Special Thanks

Um grande agradecimento ao autor original por fornecer a estrutura inicial. O ecossistema Home Assistant é movido pela colaboração!
Suporte / Support

Este add-on é fornecido "como está" para a comunidade. Para problemas específicos deste build, sinta-se à vontade para abrir uma Issue no GitHub.
Licença / License

MIT License - Copyright (c) 2026 Magus (Baseado no trabalho de Frosh)
