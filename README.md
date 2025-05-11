# 🎸 Tab AI

**Extração avançada de faixas de guitarra de vídeos do YouTube usando IA**

Ferramenta para extração de faixas instrumentais de guitarra de vídeos do YouTube utilizando modelos de separação musical baseados em IA. A versão do python recomendada é a 3.12.x

## ✨ Funcionalidades

- ⬇️ Download automático de áudio do YouTube em alta qualidade
- 🧠 Separação de faixas usando modelo **HTDemucs_6s**
- 🎚️ Isolamento profissional de guitarra com preservação de qualidade
- 📂 Organização automática em estrutura de pastas intuitiva

## 📥 Instalação

1. **Pré-requisitos**
   - [FFmpeg](https://ffmpeg.org/)
   - Python 3.8+

```bash
# Windows
choco install ffmpeg

# Linux
sudo apt install ffmpeg

# Mac
brew install ffmpeg
```

2. **Clonar o repositório**

```bash
git clone https://github.com/ericklaus16/Tab-AI
cd Tab-AI
```

3. **Criar ambiente virtual**

```bash
python -m venv venv

./venv/Scripts/activate
```

4. **Instalar dependências**

```bash
pip install yt-dlp demucs torchaudio

# ou

pip install -r requirements.txt
```

## 🚀 Como usar

1. **Execute o script main.ipynb**

2. **Cole a URL da música no youtube quando solicitado**

3. **Aguarde o processamento (pode demorar dependendo do hardware)**

Saída esperada:

```bash
⏬ Baixando áudio do YouTube...
🎸 Extraindo guitarra com IA... (isso pode demorar)
✅ Extração concluída! Guitarra disponível em:
output/Nome_do_Vídeo/guitar.mp3
```

## 📂 Estrutura de Arquivos

```bash
output/
└── Nome do Vídeo/
    └── guitar.mp3      # Faixa de guitarra isolada
    └── bass.mp3        # Faixa do baixo isolada
    └── drums.mp3       # Faixa da bateria isolada
    └── other.mp3       # Faixa de outros instrumentos isolada
    └── piano.mp3       # Faixa do piano isolada
    └── vocals.mp3      # Faixa dos vocais/backing vocals isoladas
```