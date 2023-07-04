# diachronic-Chinese-tracking

## sense-context dataset: 

contains 265289 words (including 8996 characters), 412529 senses (including 55080 senses for characters), and 856273 contexts, extracted from the Great Chinese Dictionary (汉语大词典、汉语字典) 
 
### senses.json:

word: word name;  
wsid: the ID of sense;   
newgloss: definations of the sense from dictionary, we simplified it ("家畜名。俗称狗。为人类最早驯化的家畜之一。听觉、嗅觉灵敏。性机警，易于训练。品种很多，按用途可分为牧羊犬、猎犬、警犬、玩赏犬以及挽曳犬、皮肉用犬等。" ---->  "家畜名,狗")    

e.g.  
{
            "word": "犬",
            "wsid": "496940",
            "newgloss": "家畜名,狗"
        },
        {
            "word": "犬",
            "wsid": "496941",
            "newgloss": "为自谦或鄙斥他人之词"
        },

### contexts.json:


{
            "artid": "988259",
            "txt": "雨后有人耕绿野，月明无犬吠花村。",
            "age": "6",
            "wsid": "496940",
            "article": "救风尘",
            "title": "救风尘",
            "author": "元关汉卿"
        },
