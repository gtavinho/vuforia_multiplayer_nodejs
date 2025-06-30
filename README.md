# 🎮 Sistema Multijogador com NodeJS
Aplicação do recurso multiplayer via nodejs em um ambiente de realidade aumentada com Vuforia / Unity3D para Android
# 

> Projeto de jogo multiplayer em tempo real utilizando Unity3D (cliente) e Node.js (servidor)

## 📋 Índice

1. [Sobre o Projeto](#sobre-o-projeto)
2. [Compilação do Cliente (Unity3D)](#compilação-do-cliente-unity3d)
3. [Instalação do Cliente no Android](#instalação-do-cliente-no-android)
4. [Configuração do Servidor (NodeJS)](#configuração-do-servidor-nodejs)
5. [Requisitos Mínimos](#requisitos-mínimos)
6. [Como Contribuir](#como-contribuir)
7. [Licença](#licença)

---

## 🧾 Sobre o Projeto

Este projeto tem como objetivo implementar um sistema multiplayer em tempo real usando **Unity3D** como cliente gráfico e **Node.js** como servidor responsável pela comunicação entre os jogadores.

Ele utiliza tecnologia de reconhecimento de imagem para ativar o ambiente 3D ao apontar a câmera do dispositivo móvel para uma imagem referência impressa.

---

## 🔨 Compilação do Cliente (Unity3D)

### Passo a passo:

1. **Abra o projeto no Unity3D**
   - Utilize a versão mais recente ou compatível com o projeto.

2. **Configure o IP do servidor:**
   - Navegue até o script `Network.cs` dentro da pasta `Assets`.
   - Selecione o script no painel de inspetor.
   - Localize o grupo chamado **Socket IO Component**.
   - No campo **Url**, insira o endereço IP do servidor que deseja conectar:
     ```
     http://<IP_DO_SERVIDOR>:3000
     ```

3. **Compile o projeto:**
   - Vá para `File > Build & Run`.
   - Escolha a plataforma desejada (ex.: **Android**).
   - Clique em **Build**.
   - Selecione uma pasta para salvar o arquivo `.apk`.
   - Confirme o salvamento.

---

## 📱 Instalação do Cliente no Android

### Requisitos mínimos:

- Sistema operacional: **Android 4.4 ou superior**
- Memória RAM: **512 MB**
- Armazenamento interno: **200 MB**

### Passos para instalação:

1. Transfira o arquivo `.apk` gerado (`Projeto_TCC2_nodejs.apk`) para o dispositivo Android.
2. Acesse **Configurações > Segurança**.
3. Ative a opção **Fontes desconhecidas** para permitir instalação de apps fora da Play Store.
4. Abra o arquivo `.apk` através do gerenciador de arquivos.
5. Toque em **Instalar** e siga as etapas.
6. Após instalado, localize o ícone do aplicativo em **Aplicativos** e execute-o.

### Como usar:

1. Imprima a imagem fornecida (**Figura 03**) em tamanho A4.
2. Execute o app.
3. Aponte a câmera do celular para a imagem impressa para ativar o ambiente 3D.

---

## ⚙️ Configuração do Servidor (NodeJS)

### Passo a passo:

1. **Baixe e instale o Node.js**
   - Acesse: https://nodejs.org/en/download/
   - Recomenda-se a versão **LTS** ou a mais recente.

2. **Navegue até a pasta do servidor:**
   - Abra o terminal (ou prompt de comando).
   - Acesse a pasta `server` localizada na raiz do projeto:
     ```bash
     cd caminho/para/o/projeto/server
     ```

3. **Instale as dependências:**
   ```bash
   npm install
   ```

4. **Inicie o servidor:**
   ```bash
   node server.js
   ```

> O servidor rodará na porta padrão `3000`. Certifique-se de que essa porta esteja liberada no firewall.

---

## 🧰 Requisitos Mínimos

| Componente | Requisito |
|------------|-----------|
| 📲 Dispositivo Android | Versão 4.4 ou superior |
| 💾 Memória RAM (Cliente) | 512 MB |
| 🗃️ Armazenamento Interno (Cliente) | 200 MB |
| 🖥️ Sistema Operacional (Servidor) | Qualquer SO compatível com Node.js |
| 🟩 Node.js | Versão mais recente ou LTS |

---

## 🤝 Como Contribuir

Se quiser contribuir com esse projeto, fique à vontade! Você pode:

- Corrigir bugs
- Melhorar a documentação
- Adicionar novas funcionalidades
- Traduzir para outros idiomas

Basta seguir estas etapas:

1. Faça um fork do repositório
2. Crie uma nova branch (`git checkout -b feature/nova-feature`)
3. Faça commit das suas alterações (`git commit -m 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/nova-feature`)
5. Abra um Pull Request

---

## 📄 Licença

Este projeto está licenciado sob a **MIT License**. Veja o arquivo `LICENSE` para mais informações.

---

Se precisar de uma tradução para inglês, adição de imagens, badges do GitHub ou integração com ferramentas como Docker, posso ajudar também! Deseja alguma personalização adicional?
