# Emoji-Detection-
This is a project which detect the emoji.
import emot

em = emot.core.emot()
text = "Hello 😊 world! :-)"
print(em.emoji(text))
# → {'value': ['😊'], 'location': [[6,7]], ... }
print(em.emoticons(text))
# → {'value': [':-)'], ... }
git clone https://github.com/TetsumichiUmada/text2emoji.git
cd text2emoji
pip install -r requirements.txt
jupyter notebook project.ipynb
git clone https://github.com/iMalakAhmed/Emoji-Detection-System.git
cd Emoji-Detection-System
pip install -r requirements.txt
# Download the FER‑2013_sampled data as instructed
python train.py --data-dir FER-2013_sampled
python inference.py --model models/emoji_mlp.pkl
