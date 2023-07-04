# diachronic-Chinese-tracking

## sense-context dataset: 

contains 265289 words (including 8996 characters), 412529 senses (including 55080 senses for characters), and 856273 contexts, extracted from the Great Chinese Dictionary (汉语大词典、汉语字典) 
 
### senses.json:

word: word of sense;  
wsid: the ID of sense;   
newgloss: definations of the sense from dictionary, we simplified it (e.g. "家畜名。俗称狗。为人类最早驯化的家畜之一。听觉、嗅觉灵敏。性机警，易于训练。品种很多，按用途可分为牧羊犬、猎犬、警犬、玩赏犬以及挽曳犬、皮肉用犬等。" ---->  "家畜名,狗")    

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

artid: ID of context;  
txt: context;     
age: time of context (1-10: please see Time ranges);  
wsid: the ID of sense;   
article, title: first level title, second level title;  
author: author information  

#### Time ranges: we divided time intervals by Chinese dynasties  

 

1  先秦 pre-Qin        （<221BC)   
2  秦汉 Qin & Han        （221BC - 220AD）    
3  魏晋南北朝  Wei,Jin,Southern and Northern   （220AD - 581AD）     
4  隋唐 Sui & Tang    （581AD - 960AD）    
5  宋 Song              （960AD - 1279AD）    
6  元 Yuan              （1279AD - 1368AD）  
7  明 Ming              （1368AD - 1644AD）    
8  清 Qing              （1644AD - 1840AD）   
9  近 recent era          （1840AD - 1919AD）  
10 当  contemporary era            （1919AD<）                                      

( Time ranges for sense-context dataset and historical literature corpus were annotated by automatically searching Baidu Baike based on their author and title)


e.g.  
{
            "artid": "988259",
            "txt": "雨后有人耕绿野，月明无犬吠花村。",
            "age": "6",
            "wsid": "496940",
            "article": "救风尘",
            "title": "救风尘",
            "author": "元关汉卿"
        }, 



## historical literature corpus:

contains 4569 documents distributed throughout various dynasties  
extracted from the Daizhige corpus, deleting the duplicate documents and that were failed to find dynasty  
Daizhige corpus: https://github.com/garychowcmu/daizhigev20  


 ### corpus_t1 - corpus_t10:  
 we organized documents according to the time range（1-10） 
 

 
