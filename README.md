# 🔐 Trabalho 9XMJ: Desafio de Engenharia Reversa

> ⚠️ **ATENÇÃO: esta é uma atividade de alta dificuldade e vale a nota do ano inteiro.**
> **Quem não conseguir concluir o desafio estará reprovado.**

---

## 🚦 Antes de começar

1. **Isole o ambiente**: rode o `trabalho_escola_9xmj.exe` apenas dentro de uma máquina virtual.
2. **Desative a internet/rede** dessa VM antes de executar o arquivo pela primeira vez.
3. **Tire um snapshot** da VM limpa, assim você pode restaurar o estado sempre que precisar testar algo novo.
4. Só então comece a **planejar sua estratégia de ataque**: o que observar primeiro, quais ferramentas usar, como documentar cada descoberta.

## 📌 Sobre o desafio

Este repositório contém o `trabalho_escola_9xmj.exe`, um aplicativo criado pelo professor em ambiente controlado, exclusivamente para fins educacionais. A tela de login e a validação de usuário/senha são **totalmente locais**, embutidas no próprio binário — o app **não se conecta à internet nem a nenhum servidor**.

Sua missão é aplicar na prática o que foi aprendido em engenharia reversa para **burlar a tela de login e chegar ao menu principal** da aplicação.

📦 Arquivo do desafio: [`trabalho_escola_9xmj.exe`](https://github.com/EMAN0OEL/Trabalho_9XMJ/blob/main/trabalho_escola_9xmj.exe)

## 🎯 Objetivo

Contornar a verificação de usuário e senha (seja descobrindo as credenciais corretas, seja aplicando um patch no binário) e conseguir acessar o menu principal do aplicativo.

## ⚙️ Importante sobre o funcionamento do app

- Todo o processo de autenticação acontece **localmente**, dentro do próprio executável.
- O aplicativo **não faz nenhuma requisição de rede** — não se conecta a servidores, bancos de dados externos ou internet.
- Isso significa que toda a lógica necessária para resolver o desafio pode ser encontrada **dentro do próprio binário**, usando engenharia reversa estática e dinâmica.

## 🛠️ Ferramentas sugeridas

- Ghidra / IDA Free / Binary Ninja
- x64dbg / OllyDbg
- Detect It Easy (DIE)
- `strings`, PE-bear, Process Monitor

## 🧪 Regras e segurança

1. **Execute o `trabalho_escola_9xmj.exe` somente dentro de uma máquina virtual**, com a rede/internet **desativada** (snapshot antes de rodar).
2. Não execute o arquivo na sua máquina principal.
3. O trabalho é **individual**. [ou: em grupos de até X alunos]
4. É proibido copiar soluções de colegas ou de terceiros.
5. O uso das técnicas aprendidas é restrito a este desafio e a ambientes autorizados.

## 📤 Entrega

Envie para o professor até **HOJE**:

- Um **relatório** descrevendo, passo a passo, como você chegou à solução (ferramentas usadas, análise estática/dinâmica, raciocínio)
- Prints ou gravação mostrando o acesso ao menu principal
- [Keygen/patch, se aplicável]

## 📊 Critério de avaliação

| Resultado | Situação |
|---|---|
| Desafio concluído com relatório válido | ✅ Aprovado |
| Desafio não concluído | ❌ Reprovado |

## 💡 Dicas

- Comece pela análise estática: strings, imports e estrutura geral do binário.
- Depois, use o debugger para observar o comportamento em tempo de execução na tela de login.
- Anote tudo o que descobrir. O relatório faz parte da entrega.

---

**Boa sorte! 🍀**
