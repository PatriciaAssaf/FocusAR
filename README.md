FOCUSAR — Pomodoro em Realidade Aumentada
LEIA-ME.txt

SOBRE O PROJETO

FocusAR é um temporizador Pomodoro desenvolvido em Realidade Aumentada, criado como projeto final 
do curso de Capacitação em Realidade Aumentada.

A aplicação sobrepõe uma interface 3D interativa ao mundo real por meio do marcador Hiro, permitindo 
que o usuário gerencie sessões de foco diretamente pela câmera do celular, sem necessidade de instalação.

Esta versão representa um MVP com as funcionalidades essenciais implementadas e funcionais. O projeto
foi concebido com escopo maior e deverá ser incrementado em versões futuras, conforme descrito na seção 
"Próximos Passos".

Autora : Patricia Mahmoud Assaf
Curso  : Capacitação em Realidade Aumentada


LINK PÚBLICO (Netlify): thunderous-chimera-3046f7.netlify.app


COMO USAR

1. Acesse o link público
2. Permita o acesso à câmera quando solicitado
3. Imprima ou exiba o marcador Hiro e aponte a câmera para ele
4. Toque UMA VEZ na tela para iniciar ou pausar o timer
5. Toque DUAS VEZES rapidamente na tela para resetar o timer

Marcador Hiro disponível em:
https://ar-js-org.github.io/AR.js/data/images/hiro.png


FUNCIONALIDADES IMPLEMENTADAS

- Timer Pomodoro de 25 minutos de foco
- Controle por toque único (iniciar/pausar) e duplo toque (resetar)   sem necessidade de acertar 
botões específicos na tela
- Modelo 3D com botões visuais sobrepostos ao marcador Hiro
- Estados exibidos em tempo real: FOCO, PAUSADO e FINALIZADO
- Alerta sonoro ao fim da sessão (3 bipes gerados via Web Audio API, sem necessidade de arquivo de áudio externo)
- Publicado e funcional em dispositivos móveis


PRÓXIMOS PASSOS (versões futuras)

Este projeto foi entregue em sua versão inicial funcional. As funcionalidades abaixo foram planejadas 
e fazem parte do escopo completo do FocusAR, a ser desenvolvido posteriormente:

- Ciclo completo Pomodoro: alternância automática entre sessões   de foco (25 min) e pausas curtas (5 min) 
e longas (15 min)
- Contador de ciclos concluídos exibido na cena 3D
- Animação de progresso visual (círculo preenchendo conforme o tempo avança)
- Vibração do dispositivo ao fim de cada sessão
- Configuração de tempo diretamente na interface AR


ARQUIVOS DO PROJETO

index.html          → código principal da aplicação
FocusAR2teste.glb   → modelo 3D da interface (botões e círculo)
LEIA-ME.txt         → este arquivo


CRÉDITOS E TECNOLOGIAS

Modelo 3D
  Autoral, criado no Blender pela autora do projeto. Não disponível em repositório externo.

Marcador
  Padrão Hiro — fornecido pela biblioteca AR.js
  https://ar-js-org.github.io/AR.js

Áudio
  Gerado via Web Audio API do navegador.   Nenhum arquivo de áudio externo foi utilizado.

A-Frame 1.3.0
  Biblioteca de WebAR/WebVR — Licença MIT
  https://aframe.io

AR.js
  Biblioteca de Realidade Aumentada para web — Licença MIT
  https://ar-js-org.github.io/AR.js


OBSERVAÇÕES TÉCNICAS

- O som é ativado somente após o primeiro toque na tela, por restrição dos navegadores mobile 
(política de autoplay de áudio).
- Para melhor rastreamento do marcador, use ambiente bem iluminado.
- Testado no Chrome para Android.
