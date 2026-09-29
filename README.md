# 🏥 Totem de Senhas – HMCC (Protótipo)

Protótipo de um totem de autoatendimento para retirada de senhas no **Hospital Municipal Carlos Chagas (HMCC)**.

O paciente toca na tela, escolhe o serviço (ou fala o que precisa) e recebe uma senha na hora. O totem foi pensado para ser **simples de usar**, com botões grandes, poucas telas e ajuda por voz.

> ⚠️ Este é um projeto de estudo. Ele ainda não está ligado a um sistema real do hospital.

---

## ✨ O que ele faz

- Tela de boas-vindas com um botão grande para começar
- Pergunta em voz alta: **"Precisa de ajuda?"**
- **Ajuda por voz:** o paciente fala o serviço e o totem escolhe sozinho
- Menu com botões para escolher o serviço, se preferir tocar
- Gera a senha com sigla e número (exemplo: `PR01`), o nome do serviço, a data e a hora
- A contagem de senhas de cada serviço recomeça a cada novo dia
- Depois de 7 segundos, o totem volta para a tela inicial

---

## 📂 Versões

O projeto tem duas versões, cada uma com um tipo de atendimento:

| Arquivo | Para que serve | Serviços |
|---|---|---|
| `Totem1.html` | Atendimento por **prioridade** | Preferencial (+60), Super Preferencial (+80), Teste de orelhinha, Gestante C.O, Procedimento Cirúrgico, Vítima de Violência Sexual |
| `Totem2.html` | Atendimento por **especialidade** | 20 especialidades, como Cardiologia, Pediatria, Ortopedia e Neurologia, com botões de página (⬅️ ➡️) |

---

## ▶️ Como usar

1. Baixe os arquivos `Totem1.html` e `Totem2.html`.
2. Abra o arquivo no navegador (dois cliques ou botão direito > Abrir com).
3. Permita o uso do **microfone** quando o navegador pedir.

Não precisa instalar nada.

**Recomendado:** Google Chrome ou Microsoft Edge. A ajuda por voz pode não funcionar em outros navegadores.

---

## 🛠️ Tecnologias

- **HTML** e **CSS** para as telas
- **JavaScript** para a lógica do totem
- **Web Speech API** para falar (`SpeechSynthesis`) e para ouvir (`SpeechRecognition`)
- **localStorage** para guardar a contagem das senhas no navegador

---

## ⚠️ Limitações

- A senha aparece só na tela, ainda **não é impressa**.
- A contagem fica salva **apenas naquele navegador**. Se abrir em outro computador, começa do zero.
- O reconhecimento de voz depende do navegador e, em alguns casos, de internet.
- Não existe painel de chamada nem sistema de atendimento ligado ao totem.

---

## 🚀 Ideias para melhorar

- Imprimir a senha em uma impressora térmica
- Guardar as senhas em um banco de dados, para vários totens usarem a mesma contagem
- Criar um painel que mostre e chame as senhas
- Evitar siglas repetidas no `Totem2` (Nefrologia e Neurologia hoje geram a mesma sigla `NE`)
- Mostrar só a sigla na senha dos atendimentos sensíveis, para proteger a privacidade do paciente
- Juntar as duas versões em um único totem

---

## 👩‍💻 Autora

**Andressa** – estudante de Engenharia Elétrica (Unifei) e Ciência de Dados (Uninter).
