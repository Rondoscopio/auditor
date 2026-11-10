# Análise temporal, contexto e interpretação responsável

Este documento registra diretrizes e requisitos conceituais para o Córtex, sistema de análise e inteligência investigativa do Rondoscópio. São propostas em planejamento, não funcionalidades implementadas.

## Limites da evidência e da interpretação

Uma evidência isolada pode sustentar fatos pontuais, mas não autoriza automaticamente conclusões sobre intenção, motivação, veracidade, causalidade, favorecimento ou responsabilidade. Mesmo um conjunto de documentos requer verificação do contexto e de explicações alternativas.

A análise deve distinguir:

1. **Registro:** o arquivo, a publicação ou a observação preservada, com sua proveniência e limitações.
2. **Acontecimento:** o fato reconstruído a partir dos registros, incluindo incertezas e divergências.
3. **Contexto:** antecedentes, consequências, participantes, circunstâncias e informações que podem alterar o sentido.
4. **Interpretação:** hipótese ou conclusão fundamentada, identificando evidências favoráveis, contrárias e lacunas.

Nem toda afirmação registrada é verdadeira, nem toda ocorrência cronológica comprova relação causal.

## Interpretação temporal e mudança de posicionamento

O sistema deve permitir examinar declarações e ações em sequência, sem assumir que uma frase isolada representa a posição definitiva de alguém. A análise de possível contradição exige considerar:

- Ironia, sarcasmo, humor, citações e falas hipotéticas.
- Trechos cortados, contexto original e autoria efetiva.
- Correções, retratações, mudanças legítimas de opinião e fatos novos.
- Diferenças entre promessas, intenções declaradas, votos, atos administrativos e efeitos observados.
- Transformações de papel institucional, competência, circunstâncias e legislação aplicável.
- Possíveis incentivos e conflitos de interesse, sem presumir motivação por mera associação.

Uma mudança de opinião não equivale necessariamente a má-fé. A aparente coerência de discursos tampouco comprova coerência das ações. A avaliação deve permitir hipóteses concorrentes, revisão humana, contestação e direito de resposta.

## Relevância retrospectiva e relações descobertas depois

Um registro aparentemente trivial pode adquirir relevância anos após a coleta. Um nome ou logotipo de patrocinador em fotografia antiga, por exemplo, pode ajudar a reconstruir uma relação com uma empresa que posteriormente contrata com o poder público.

Essa descoberta justifica uma pergunta investigativa e não comprova, por si só, favorecimento. Será necessário verificar o patrocínio, a identidade da empresa, as pessoas envolvidas, a natureza e o período das relações, a competência decisória, os procedimentos de contratação, a concorrência, o contexto econômico e explicações alternativas.

O Córtex deve permitir buscar retrospectivamente no acervo da [Amnésia](https://github.com/Rondoscopio/amnesia/blob/main/docs/captura-proveniencia-e-preservacao.md), inclusive por:

- Nomes atuais e históricos, razão social, nomes de fantasia e alterações societárias.
- Logotipos, marcas antigas, texto presente em imagens, documentos e vídeos.
- Menções em áudios, transcrições, atas, publicações, contratos e notícias.
- Eventos, participações, patrocínios, decisões, benefícios, vínculos e agentes públicos.
- Registros com datas próximas ou distantes e relações que só se tornaram identificáveis depois.
- Evidências contraditórias, documentos ausentes e hipóteses descartadas.

## Modelo relacional e temporal

Avaliar um modelo de eventos e grafo de conhecimento com identificação de entidades, relações tipadas e referências à evidência de origem. Cada relação relevante deve, quando disponível, indicar:

- Entidades envolvidas, tipo de vínculo, papel exercido e contexto.
- Fonte ou fontes que justificam a ligação e forma de extração da informação.
- Data em que o acontecimento ocorreu, intervalo de validade da relação, data do registro e data em que a informação foi conhecida.
- Situação de verificação e grau de confiança, com incerteza explicitada.
- Mudanças, término de vínculos, retificações, homônimos e hipóteses de identidade não confirmadas.
- Versões de interpretações, revisões realizadas e motivos das alterações.

Evitar tratar uma fotografia de duas pessoas como prova de amizade duradoura, ou uma presença em evento como participação decisória. Um patrocinador identificado numa imagem não é automaticamente beneficiário de ato administrativo futuro.

Considerar separadamente o tempo do acontecimento e o tempo de conhecimento do registro. Esse cuidado ajuda a evitar anacronismos e conclusões construídas com fatos que ainda não eram conhecidos à época.

## Análise multivariada, tensores e aprendizagem de máquina

Séries temporais, grafos temporais, representações vetoriais e tensoriais podem ajudar a modelar padrões que envolvem múltiplas dimensões, como pessoas, organizações, atos, locais, temas e períodos.

Essas técnicas devem ser avaliadas segundo uma pergunta investigativa concreta. A adoção de tensores não é requisito inicial, nem substitui dados originais, proveniência e explicabilidade. Representações derivadas precisam guardar ligação com as evidências que as originaram, assim como a versão dos modelos e as configurações utilizadas.

Detecções automatizadas podem priorizar verificações, mas não estabelecer culpa. Correlação, proximidade em grafos, similaridade de embeddings e coincidência temporal não demonstram causalidade ou ilicitude.

## Fluxo proposto de análise

1. Receber referências aos registros preservados na Amnésia sem modificar os originais.
2. Extrair entidades e acontecimentos como candidatos sujeitos a validação.
3. Resolver identidades com atenção a homônimos, mudanças de nome e falsos positivos.
4. Organizar relações e eventos em cronologias verificáveis.
5. Gerar perguntas e hipóteses, incluindo explicações alternativas.
6. Reunir evidências favoráveis e contrárias e assinalar lacunas.
7. Submeter achados sensíveis à revisão humana e à avaliação jurídica apropriada.
8. Registrar conclusões graduadas, incertezas, fontes, contestação e retificações.
9. Reprocessar e reexaminar casos quando novas evidências surgirem, mantendo o histórico das análises.

## Salvaguardas e critérios de qualidade

- Separar fato observado, afirmação de terceiros, inferência automatizada, hipótese e conclusão.
- Não transformar pontuações de risco, grafos ou classificadores em juízos automáticos de irregularidade.
- Distinguir ausência de evidência de evidência de ausência.
- Testar sensibilidade a fontes incompletas, enviesamento de seleção e erros de extração.
- Considerar a independência e a confiabilidade das fontes antes de tratar repetições como corroboração.
- Permitir explicações alternativas e registrar decisões de não confirmação ou descarte de hipóteses.
- Respeitar limites legais de acesso, proteção de dados, integridade e direitos de resposta.
- Não publicar dados sensíveis ou associações potencialmente danosas sem revisão proporcional.
- Preservar o histórico de correções de modo auditável e sem reescrever os registros de origem.

## Cenário ilustrativo

Uma fotografia capturada anos atrás contém o nome de uma empresa entre os patrocinadores de um evento. Em período posterior, aparecem registros públicos de interações com agentes públicos. Anos depois, a mesma empresa vence uma licitação.

O Córtex pode vincular os três acontecimentos e produzir uma cronologia acompanhada das fontes. O sistema não deve concluir favorecimento sem examinar o procedimento licitatório, a identidade dos participantes, a natureza das relações, os poderes decisórios, possíveis explicações lícitas e informações contrárias à hipótese.

O resultado correto pode ser a confirmação de uma relação, a identificação de uma questão que merece aprofundamento ou a conclusão de que os dados não sustentam suspeita de irregularidade.

## Integração com a Amnésia

A [Amnésia](https://github.com/Rondoscopio/amnesia/blob/main/docs/captura-proveniencia-e-preservacao.md) registra o material e seus metadados técnicos, inclusive proveniência de conexões e resultados de processamento. O Córtex examina padrões e contextos, relaciona fatos ao longo do tempo e revisa interpretações. Ambos devem preservar referências verificáveis entre observações, transformações e conclusões.
