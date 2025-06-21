# EasyControlDesktop

Bem-vindo ao repositório oficial do **EasyControlDesktop**, a solução para controle de dispositivos residenciais e empresariais, como tomadas, lâmpadas, ar-condicionados e muito mais, diretamente do seu computador. Este repositório é dedicado ao download do aplicativo desktop, disponível para Windows, macOS e Linux.

## 📖 Sobre o Projeto

O **EasyControl** é uma plataforma de automação que permite gerenciar dispositivos inteligentes de forma intuitiva e eficiente. Seja em casa ou em ambientes corporativos, o aplicativo desktop oferece uma interface amigável para monitorar e controlar dispositivos conectados, proporcionando conforto, economia de energia e segurança.

### 🎯 Contexto

O EasyControl foi projetado para simplificar a interação com dispositivos IoT (Internet das Coisas), como:
- **Tomadas inteligentes**: Ligue/desligue aparelhos remotamente.
- **Lâmpadas conectadas**: Ajuste intensidade, cor e programação.
- **Ar-condicionados**: Controle temperatura e modos de operação.
- Outros dispositivos compatíveis com protocolos de automação.

Com uma arquitetura robusta, o EasyControl integra dispositivos embarcados a uma interface desktop moderna, oferecendo uma experiência unificada para usuários finais.

### 🛠️ Tecnologias Utilizadas

O EasyControl é construído com tecnologias de ponta para garantir desempenho, escalabilidade e confiabilidade:
- **Electron**: Framework para desenvolvimento do aplicativo desktop multiplataforma.
- **Next.js**: Framework React para interfaces web dinâmicas e performáticas.
- **HeroUI**: Biblioteca de componentes para uma interface visual consistente e moderna.
- **MQTT**: Protocolo de comunicação leve para troca de dados com dispositivos IoT.
- **WebSocket**: Comunicação em tempo real para atualizações instantâneas.
- **Node.js**: Backend robusto para integração e processamento.
- **C++**: Utilizado nos sistemas embarcados para controle eficiente dos dispositivos.

## 📥 Como Baixar e Instalar

1. **Acesse os Releases**:
   - Vá para a seção [Releases](https://github.com/seu-usuario/EasyControlDesktop/releases) deste repositório.
   - Baixe o instalador correspondente ao seu sistema operacional:
     - **Windows**: `EasyControl-Setup.exe`
     - **macOS**: `EasyControl.dmg`
     - **Linux**: `EasyControl.AppImage` ou pacote `.deb`/`.rpm`

2. **Instale o Aplicativo**:
   - **Windows**: Execute o `.exe` e siga as instruções do instalador.
   - **macOS**: Arraste o `EasyControl.app` para a pasta **Aplicativos**.
   - **Linux**: Execute o `.AppImage` ou instale o pacote `.deb`/`.rpm` conforme sua distribuição.

## 🛑 Nota para Usuários de macOS

O EasyControl ainda não está assinado ou notarizado pela Apple, pois estamos em processo de obtenção do certificado de desenvolvedor. Se você encontrar o erro **"EasyControl está danificado e não pode ser aberto"**, siga estas instruções temporárias para executar o aplicativo:

1. **Abrir via Configurações**:
   - Após tentar abrir o app, vá em ** > Configurações do Sistema > Privacidade e Segurança** (ou **Preferências do Sistema > Segurança e Privacidade > Geral** em versões mais antigas).
   - Clique em **Abrir Mesmo Assim** na seção de segurança, se disponível.
2. **Remover Restrição via Terminal**:
   - Abra o **Terminal** e execute:
     ```bash
     sudo xattr -r -d com.apple.quarantine /Applications/EasyControl.app
     ```
   - Insira sua senha de administrador e tente abrir o app novamente.
3. **Alternativa Avançada**:
   - Desative temporariamente as restrições do sistema com:
     ```bash
     sudo spctl --master-disable
     ```
   - Após usar o app, reative a segurança com:
     ```bash
     sudo spctl --master-enable
     ```

**Aviso**: Estas são soluções temporárias. Estamos trabalhando para fornecer uma versão assinada e notarizada em breve, eliminando a necessidade desses passos.

## 🚀 Primeiros Passos

1. **Configurar Dispositivos**:
   - Certifique-se de que seus dispositivos (tomadas, lâmpadas, etc.) estão conectados à mesma rede do computador.
   - Consulte o manual dos dispositivos para obter credenciais MQTT ou WebSocket, se necessário.

2. **Explorar a Interface**:
   - Acesse a **Dashboard > Início** para uma visão geral dos dispositivos conectados.
   - Use o **Sidebar** para navegar entre seções, com o item selecionado destacado na **Navbar**.

3. **Personalizar**:
   - Configure rotinas de automação, como ligar lâmpadas ao anoitecer ou ajustar o ar-condicionado com base na temperatura.

## 🐛 Problemas Conhecidos e Suporte

- **macOS**: Erro "danificado" (veja a seção acima para soluções).
- Para outros problemas, abra uma [Issue](https://github.com/seu-usuario/EasyControlDesktop/issues) neste repositório, descrevendo o erro e seu sistema operacional.
- Consulte a [Documentação](https://seu-site.com/docs) (se disponível) ou entre em contato via [e-mail](mailto:suporte@easycontrol.com) para suporte.

## 📢 Notas de Lançamento

Consulte as [Notas de Lançamento](https://github.com/seu-usuario/EasyControlDesktop/releases) para detalhes sobre atualizações, correções e novidades.

## 🤝 Contribuições

Este repositório é voltado para distribuição do aplicativo. Para sugestões ou feedback, use a seção de [Issues](https://github.com/seu-usuario/EasyControlDesktop/issues) ou entre em contato diretamente.
