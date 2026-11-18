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

## Técnicas

Oposto direto; evitar o problema; erro comum; falso caminho; exagero/ironia; segmentação; redução de escopo; inversão de valor; contexto emocional ou moral; estudo de caso/comparação.

A entrega inclui revisão e seleção de hipóteses para teste. Pode acrescentar até duas técnicas extras quando realmente ampliarem o repertório.

## Origem e escopo

Adaptação operacional de um prompt fornecido pelo usuário e atribuído a David Deutsch. O [prompt de origem](references/prompt-original.md) está preservado como referência; não se afirma reprodução oficial de obra do autor.

A skill é independente de marca e setor. Não publica anúncios nem administra campanhas. Dados, depoimentos, descontos e condições não são inventados para completar os formatos.

## Arquivos

- [SKILL.md](SKILL.md): instruções e coleta obrigatória do briefing.
- [agents/openai.yaml](agents/openai.yaml): metadados de interface.
- [references/prompt-original.md](references/prompt-original.md): texto de origem e esclarecimento de insumos.
