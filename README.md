<p align="center">
  <a href="https://ag.tavardt.com/pt/">
    <img src="https://ag.tavardt.com/img/tavardt-banner.png" alt="TAVARDT" width="1024" />
  </a>
</p>

# Verificador e Auditor de SEO Mobile

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Verificador SEO Mobile](https://img.shields.io/badge/TAVARDT-Mobile%20SEO-5b3cf5.svg)](https://tools.tavardt.com/pt/verificador-seo-mobile/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

Auditoria de prontidao para indexacao mobile-first, diretivas de viewport, largura fixa, legibilidade tipografica e ergonomia de toque.

***

## Vetores de Risco e Impacto Operacional na Experiencia Mobile

Paginas sem configuracao adequada de viewport sao reprovadas na indexacao mobile-first do Google e perdem posicoes organicas em Portugal. Falhas de responsividade provocam quebra de layout e exigem rolamento horizontal desconfortavel para o utilizador.

Bloquear o zoom do utilizador viola normas internacionais de acessibilidade e prejudica quem necessita de ampliacao visual. Larguras fixas rigidas e fontes diminutas aumentam a taxa de rejeicao e afetam a retencao nos portais.

***

## Capacidades Centrais de Auditoria Tecnica

* **Analise de Diretiva Viewport**: Inspeciona a presenca da meta tag, largura de dispositivo, escala inicial e bloqueio de zoom, deduzindo ate 45 pontos se ausente.
* **Deteccao de Rolamento Horizontal**: Identifica declaracoes CSS de largura fixa superiores a 450px que extrapolam o viewport dos smartphones modernos.
* **Auditoria de Legibilidade Tipografica**: Rastreador de tamanhos de fonte inferiores a 12px, penalizando textos ilegiveis em ate 15 pontos.
* **Quantificacao de Alvos de Toque**: Mapeia hiperligacoes, botoes e campos de formulario para avaliar a ergonomia e densidade de interacao em ecras tateis.
* **Validacao de Icone de Toque (Apple Touch Icon)**: Verifica a declaracao do icone dedicado na seccao head do HTML, deduzindo 5 pontos caso ausente.
* **Indice de Ergonomia Mobile**: Computa uma pontuacao de 0 a 100 categorizada em SATISFACTORY, ADVISORY ou UNSATISFACTORY.
* **Emulacao Real de Smartphone**: Executa pedidos HTTP utilizando cabecalho User-Agent legitimo de Safari no iPhone para garantir analise fidedigna.

***

## Instalacao e Execucao

Requer Python 3.8 ou superior utilizando exclusivamente bibliotecas padrao.

```bash
git clone https://github.com/TAVARDT-Portugal/mobile-seo-tester-pt.git
cd mobile-seo-tester-pt
python mobile_seo_tester.py https://empresa.pt
```

Para gerar a saida em formato estruturado JSON em esteiras de integracao continua:

```bash
python mobile_seo_tester.py https://empresa.pt -j
```

***

## Perguntas Frequentes (FAQ Tecnico)

### 1. Qual o impacto da ausencia ou erro na meta tag viewport para o Google Mobile-First?
O Googlebot renderiza e avalia as paginas simulando integralmente o ecra de um smartphone. Sem a meta viewport configurada com device-width, o navegador carrega a visualizacao para desktop, provocando severas penalizacoes no posicionamento organico.

### 2. Por que a ferramenta penaliza o bloqueio de zoom com a diretiva user-scalable=no?
Impedir a ampliacao do ecra infringe as normas de acessibilidade da web para pessoas com dificuldades visuais. Os motores de busca classificam o bloqueio de escala como falha de usabilidade e reduzem a pontuacao geral do portal.

### 3. Como contentores com largura fixa acima de 450px prejudicam o desempenho mobile?
Elementos com largura fixa superior a 450px excedem a area visivel de ecras de telemoveis e geram rolamento lateral. Esse extravasamento quebra o layout responsivo e resulta em reprovacao automatica nos testes de compatibilidade movel.

### 4. Quais os riscos operacionais associados ao uso de fontes menores que 12px?
Textos com tamanho inferior a 12px exigem esforco excessivo para leitura em smartphones de alta densidade de pixeis. A auditoria penaliza fontes subdimensionadas para garantir leitura confortavel sem necessidade de zoom manual.

### 5. Por que e importante declarar a tag apple-touch-icon para navegacao movel?
A diretiva apple-touch-icon assegura que sistemas operativos moveis exibam icones de alta definicao ao guardar atalhos no ecra principal. A ausencia dessa hiperligacao gera icones genericos e enfraquece a presenca da marca no ecossistema mobile.

***

## Consultoria em SEO Mobile e Arquitetura Responsiva

Para projetos de grande escala e alinhamento com as diretrizes do Google Mobile-First Indexing e W3C, consulte os especialistas em engenharia da **TAVARDT**.

***

## Links Uteis

* **Portal Corporativo:** https://ag.tavardt.com/pt/
* **Suite de Diagnosticos:** https://tools.tavardt.com/pt/
* **Contacto Tecnico:** https://ag.tavardt.com/pt/contacto/

***

### Licenca
Distribuido sob a Licenca MIT. Consulte o arquivo LICENSE para termos completos.

***

© 2026 TAVARDT. Todos os direitos reservados.
