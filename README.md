# Copy Deutsch

Skill em português para gerar variações criativas de uma copy central, explorando modos diferentes de expandir seu conceito com base no prompt atribuído a David Deutsch: adição, subtração, inversão, exagero e outras transformações.

O formato detalhado do prompt pede **dez técnicas com três versões cada: 30 anúncios curtos, de uma a três linhas por anúncio**. A skill adota esse padrão e respeita outra quantidade quando definida explicitamente para a execução.

## Como usar

Depois de instalar, invoque `$copy-deutsch`. A skill começa pedindo:

| Insumo | O que informar | Exemplo do material de origem |
|---|---|---|
| **Ideia central — obrigatório** | Sua copy original ou conceito a expandir | Cole o anúncio que deseja variar |
| **Público-alvo — obrigatório** | Para quem a mensagem foi escrita | Mulheres acima de 35 anos que fizeram bariátrica nos últimos dois anos |
| **Objetivo — obrigatório** | A ação ou efeito pretendido | Gerar curiosidade e cliques para um programa alimentar de reeducação |
| **Tom desejado — obrigatório** | O estilo da abordagem | Emocional; direto e seco; irônico e provocativo |
| **Call-to-action — opcional** | A chamada para ação | “Descubra como”; deixe em branco se preferir sem CTA |

Ela aguarda os quatro insumos obrigatórios antes de criar. Se eles já estiverem explícitos no pedido, começa a geração; se faltarem alguns, pede apenas os faltantes. Contexto de outra campanha não preenche o briefing automaticamente.

Os exemplos acima ilustram como preencher os campos; a skill funciona em outros setores e não presume esse público ou essa oferta.

Você pode começar apenas com:

```text
Use $copy-deutsch e me peça os insumos necessários.
```

Ou entregar o briefing de uma vez:

```text
Use $copy-deutsch.
Ideia central/copy original: ...
Público-alvo: ...
Objetivo: ...
Tom desejado: ...
CTA (opcional): ...
```

## Instalação

Copie esta pasta para `~/.codex/skills/copy-deutsch` ou para a pasta `skills/copy-deutsch` dentro de `CODEX_HOME`, quando configurado. O arquivo `SKILL.md` deve ficar diretamente dentro da pasta `copy-deutsch`.

## Categorias e exemplos do prompt

Os exemplos abaixo reproduzem o material de origem e ilustram a construção de cada técnica; a aplicação deve usar o público e os fatos do briefing informado.

### Oposto direto

Provoca reação ao mostrar consequência negativa de não agir.

- “Quer engordar tudo de novo? Continue comendo como antes.”
- “Como recuperar todo o peso perdido (em tempo recorde).”
- “A bariátrica não funciona… se você fizer isso.”

### Evitar o problema

Apela ao medo da perda dos resultados já conquistados.

- “Como evitar o reganho de peso pós-bariátrica.”
- “O que fazer agora para não perder todo o esforço da cirurgia.”

### Erro comum

Destaca equívocos frequentes que impedem o sucesso.

- “A maioria das pessoas falha aqui após a bariátrica.”
- “Por que tomar só shakes pode te deixar ainda mais inchada.”

### Falso caminho

Quebra pressupostos que o público acredita serem verdades.

- “Dieta líquida eterna? Isso não é solução.”
- “Quem disse que comer menos é o segredo?”

### Ângulo exagerado / irônico

Usa hipérbole ou ironia para aumentar impacto emocional.

- “Fez bariátrica? Bem-vinda à parte difícil.”
- “Emagrecer é fácil… se você for um robô.”

### Segmentado

Personaliza a mensagem para um subgrupo específico dentro do público-alvo.

- “Você fez bariátrica e tem mais de 40 anos? Isso muda tudo.”
- “Homens perdem peso diferente após a bariátrica. Entenda como.”

### Redução de escopo

Diminui a barreira de entrada focando em passos menores e mais viáveis.

- “Como perder 2kg saudáveis por mês depois da cirurgia.”
- “Seu próximo 1kg pode ser o mais importante da sua vida.”

### Inversão de valor

Muda o foco do resultado para um novo valor ou medida de sucesso.

- “Pare de se pesar. Comece a se medir.”
- “Mais músculos, menos culpa.”

### Contexto emocional ou moral

Eleva a discussão para valores pessoais mais profundos.

- “Você fez isso por você. Continue por você.”
- “Culpa não emagrece. Consistência sim.”

### Estudo de caso / comparação

Usa exemplo real ou contraste para provar um ponto.

- “Ela fez bariátrica e engordou de novo — até entender isso.”
- “Compare: 2 mulheres, 2 cirurgias. Só uma manteve o peso.”

A entrega inclui revisão e seleção de hipóteses para teste. Pode acrescentar até duas técnicas extras quando realmente ampliarem o repertório.

## Origem e escopo

Adaptação operacional de um prompt fornecido pelo usuário e atribuído a David Deutsch. O [prompt de origem](references/prompt-original.md) está preservado como referência; não se afirma reprodução oficial de obra do autor.

A skill é independente de marca e setor. Não publica anúncios nem administra campanhas. Dados, depoimentos, descontos e condições não são inventados para completar os formatos.

## Arquivos

- [SKILL.md](SKILL.md): instruções e coleta obrigatória do briefing.
- [agents/openai.yaml](agents/openai.yaml): metadados de interface.
- [references/prompt-original.md](references/prompt-original.md): texto de origem e esclarecimento de insumos.
