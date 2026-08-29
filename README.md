# Jornada de Marca

A marca de um negócio construída em camadas, dentro do Claude. Cada agente faz uma
pergunta, devolve um documento, e passa o documento para o próximo.

**O site publicado:** https://rslimaeng.github.io/jornada-de-marca/

## O que tem aqui

| | |
|---|---|
| `index.html` | a home: os agentes escritos e os arquivos para baixar |
| `agentes/{n}-{nome}/` | o estudo de caso completo de cada agente, com o exercício |
| `downloads/orquestrador.md` | o Diretor de Marca, para as instruções de um Projeto do Claude |
| `downloads/time-de-especialistas.md` | as camadas escritas num arquivo só, para o conhecimento do Projeto |
| `downloads/skills/` | cada agente avulso, para `~/.claude/skills/` |

## Este repositório é saída, não fonte

**Nada aqui se edita à mão.** Os arquivos são gerados a partir das `SKILL.md` e do
system prompt, que vivem no repositório de trabalho do produto. Editar aqui faz a
correção viver num lugar só, e os artefatos passam a dizer coisas diferentes.

Para republicar depois de mudar uma fonte:

```
python3 padrao-de-construcao/compilar-time-de-especialistas.py --bolha versoes-do-produto/2-brand-8
python3 padrao-de-construcao/publicar-site.py --bolha versoes-do-produto/2-brand-8 --site site-jornada-de-marca
```

## Sobre o conteúdo

O negócio dos exemplos é fictício. Os números existem para que a conta possa ser
conferida: todos saem de uma base contábil única e aberta, e nenhum artefato
publica um número que não esteja lá.

**Conteúdo de produto, com `noindex`.** O repositório é público para o GitHub Pages
funcionar; as páginas não entram em buscador. Isso não é controle de acesso: quem
tiver o link, entra.

---

*Rafael Lima · Xquads v2 · bolha 2, Jornada de Marca*
