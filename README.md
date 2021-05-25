# Abstractive Review-Text-Summarizer

This is a seq2seq text summarizer with attention network. The dataset used is the amazon review dataset which can be found <a href='https://www.kaggle.com/snap/amazon-fine-food-reviews'>here.</a>
The model can be further improved by using bidirectional LSTM. The current training time was 19 min/epoch on colab GPU which will increase significantly with bidirectional LSTMs.
The same network can be trained with some conversational data like Samsun data in order to produce daily conversational summaries of maybe lectures, papers, books etc.

Basic preprocessing is applied on the input data and then it is tokenized and padded. After that the encoder decoder model is used.

## Sample Output

**Review**: love hot sauces rediculous thought like good hot sauce would good tacos nachos etc nice heat stuff stupid hot bought three pack regreted moment tried standard insanity sauce cannot even tolerate dashes tacos good <br>
**Original summary**: seriously <br>
**Predicted summary**:  good hot sauce<br>


Review: whenever want add bit cream soup sauce never seem around use cream often enough even buy smallest container stuff kept long time really add creamy flavor glad found <br>
**Original summary**: this stuff is great <br>
**Predicted summary**:  love this stuff<br>


**Review**: glad opportunity purchase last boxes amazing tea local herb stores tell sold anymore cannot sold unless ground powder form hope buy overseas batch runs <br>
**Original summary**: last of the best <br>
**Predicted summary**:  love this tea<br>


**Review**: tried peanut butter creme version first impression fudge coating looker rather soft would messy left warm day tasting overwhelming sweetness predominant aside sweetness flavor butterfinger reeses slight crunchiness cookie portion also made texturally similar butterfinger chocolate flavor present drowned sugar fudge coating seems chocolate flavored actual chocolate excess sweetness cookies makes hard eat one good thing considering nutritional information overall cookies much sweet taste like candy bar <br>
**Original summary**: too sweet <br>
**Predicted summary**:  not bad not great<br>

**Review**: love product kids drink instead sports drinks play soccer much healthier twice received amazon times product poorly packaged times padding cartons got crushed shipping cartons leak amazon responded well shipping replacement cartons still padding leaks would like continue buy amazon figure package cartons get crushed <br>
**Original summary**: poorly packaged <br>
**Predicted summary**:  great product poor packaging<br>

<p align=center> Made with :heart: by Bhuvan Aggarwal</p>

