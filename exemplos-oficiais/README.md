# Exemplos oficiais (Portal de Serviços do DATASUS)

Estes dois arquivos foram baixados diretamente do Portal de Serviços do DATASUS
(página de cada serviço, aba de exemplos/documentação), e servem para conferir
os defeitos nº 2 a 5 (REL) e nº 15 (SA) relatados no texto.

## exemploJSONRELv3.0.json — REL (Resultado de Exame Laboratorial)

- **Baixado em:** 14/06/2026, 17:00:02 (horário de Brasília, -03:00)
- **Origem:** `https://mobileapps.saude.gov.br/portal-servicos/files/f3bd659c8c8ae3ee966e575fde27eb58/2e79ba49d14cafef4976252823071f34_8zi01cl93.json`
  (confirmado pelo histórico de downloads do navegador; data/hora coincide com
  o `mtime` do arquivo)
- **Perfil FHIR do recurso principal** (`Composition.meta.profile`):
  `http://www.saude.gov.br/fhir/r4/StructureDefinition/BRResultadoExameLaboratorial-3.2.1`
  → versão **3.2.1** do perfil `BRResultadoExameLaboratorial`.
- **Versão do manual de integração (texto, não o perfil FHIR):** não verificada
  por mim — a página do serviço no Portal exige login/credenciamento, e eu não
  tenho acesso a essa sessão autenticada. Pendente: confirmar o número da
  versão do manual exibido na página do REL no Portal (ex.: "Manual de
  Integração REL vX.Y") e completar esta linha.

## exemploJSONSA.json — SA (Sumário de Alta)

- **Baixado em:** 19/09/2026, 22:55:18 (horário de Brasília, -03:00)
- **Origem:** `https://mobileapps-prd.saude.gov.br/portal-servicos2/files/f4bd659c8c8ae3ee966e575fde27eb58/0935c53de80e45ceec3f0800d0617c47_igpmdvp85.json`
  (confirmado pelo histórico de downloads do navegador; data/hora coincide com
  o `mtime` do arquivo)
- **Perfil FHIR do recurso principal** (`Composition.meta.profile`):
  `http://www.saude.gov.br/fhir/r4/StructureDefinition/BRSumarioAlta`
  (sem sufixo de versão no identificador do perfil — é o perfil "vigente" tal
  como publicado no Simplifier/Portal na data do download).
- **Versão do manual de integração (texto):** mesma observação do REL acima —
  não verificada por falta de acesso à página autenticada do Portal.

## Como os números de download foram confirmados

Os `mtimes` dos dois arquivos coincidem, ao segundo, com os registros de
download do Firefox (`moz_annos` / `places.sqlite`) para a URL de origem acima,
o que corrobora que estes são de fato os arquivos baixados do Portal, e não
cópias editadas manualmente.
