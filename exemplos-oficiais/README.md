# Exemplos oficiais (Portal de Serviços do DATASUS)

Estes dois arquivos foram baixados diretamente do Portal de Serviços do DATASUS
(página de cada serviço, aba de exemplos/documentação), e servem para conferir
os defeitos dos exemplos relatados no texto. No do REL estão os nº 2, 5, 6 e 8;
os nº 3 e 4 estão só no manual impresso (o `"01"` do arquivo é o código do
patógeno, e não o da suspeita diagnóstica). No do SA estão as vinte divergências
do nº 15, as mesmas do Anexo 1 do manual.

## exemploJSONRELv3.0.json — REL (Resultado de Exame Laboratorial)

- **Baixado em:** 14/06/2026, 17:00:02 (horário de Brasília, -03:00)
- **Origem:** `https://mobileapps.saude.gov.br/portal-servicos/files/f3bd659c8c8ae3ee966e575fde27eb58/2e79ba49d14cafef4976252823071f34_8zi01cl93.json`
  (confirmado pelo histórico de downloads do navegador; data/hora coincide com
  o `mtime` do arquivo)
- **Perfil FHIR do recurso principal** (`Composition.meta.profile`):
  `http://www.saude.gov.br/fhir/r4/StructureDefinition/BRResultadoExameLaboratorial-3.2.1`
  → versão **3.2.1** do perfil `BRResultadoExameLaboratorial`.
- **Versão do manual de integração (texto) usada na conferência do TCC:** 3.1,
  de 09/07/2024, a última do histórico de versões do manual. A versão exibida
  hoje na página do serviço no Portal não foi conferida, porque a página exige
  login.

## exemploJSONSA.json — SA (Sumário de Alta)

- **Baixado em:** 19/09/2026, 22:55:18 (horário de Brasília, -03:00)
- **Origem:** `https://mobileapps-prd.saude.gov.br/portal-servicos2/files/f4bd659c8c8ae3ee966e575fde27eb58/0935c53de80e45ceec3f0800d0617c47_igpmdvp85.json`
  (confirmado pelo histórico de downloads do navegador; data/hora coincide com
  o `mtime` do arquivo)
- **Perfil FHIR do recurso principal** (`Composition.meta.profile`):
  `http://www.saude.gov.br/fhir/r4/StructureDefinition/BRSumarioAlta`
  (sem sufixo de versão no identificador do perfil — é o perfil "vigente" tal
  como publicado no Simplifier/Portal na data do download).
- **Versão do manual de integração (texto) usada na conferência do TCC:** 1.0,
  com a atualização de 03/06/2026 registrada no histórico de revisões do manual.
  A versão exibida hoje no Portal não foi conferida, pelo mesmo motivo.

## Como os números de download foram confirmados

Os `mtimes` dos dois arquivos coincidem, ao segundo, com os registros de
download do Firefox (`moz_annos` / `places.sqlite`) para a URL de origem acima,
o que corrobora que estes são de fato os arquivos baixados do Portal, e não
cópias editadas manualmente.
