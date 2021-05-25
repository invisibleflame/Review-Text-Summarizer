# Abstractive Review-Text-Summarizer

This is a seq2seq text summarizer with attention network. The dataset used is the amazon review dataset which can be found <a href='https://www.kaggle.com/snap/amazon-fine-food-reviews'>here.</a>
The model can be further improved by using bidirectional LSTM. The current training time was 19 min/epoch on colab GPU which will increase significantly with bidirectional LSTMs.
The same network can be trained with some conversational data like Samsun data in order to produce daily conversational summaries of maybe lectures, papers, books etc.

Basic preprocessing is applied on the input data and then it is tokenized and padded. After that the encoder decoder model is used.

## Sample Output

Review: love hot sauces rediculous thought like good hot sauce would good tacos nachos etc nice heat stuff stupid hot bought three pack regreted moment tried standard insanity sauce cannot even tolerate dashes tacos good 
Original summary: seriously 
Predicted summary:  good hot sauce


Review: whenever want add bit cream soup sauce never seem around use cream often enough even buy smallest container stuff kept long time really add creamy flavor glad found 
Original summary: this stuff is great 
Predicted summary:  love this stuff


Review: glad opportunity purchase last boxes amazing tea local herb stores tell sold anymore cannot sold unless ground powder form hope buy overseas batch runs 
Original summary: last of the best 
Predicted summary:  love this tea


Review: tried peanut butter creme version first impression fudge coating looker rather soft would messy left warm day tasting overwhelming sweetness predominant aside sweetness flavor butterfinger reeses slight crunchiness cookie portion also made texturally similar butterfinger chocolate flavor present drowned sugar fudge coating seems chocolate flavored actual chocolate excess sweetness cookies makes hard eat one good thing considering nutritional information overall cookies much sweet taste like candy bar 
Original summary: too sweet 
Predicted summary:  not bad not great

<p align=center> Made with :heart: by Bhuvan Aggarwal</p>
Review: love product kids drink instead sports drinks play soccer much healthier twice received amazon times product poorly packaged times padding cartons got crushed shipping cartons leak amazon responded well shipping replacement cartons still padding leaks would like continue buy amazon figure package cartons get crushed 
Original summary: poorly packaged 
Predicted summary:  great product poor packaging


Review: delicious coffee ever drink hot cold drink cold litle cream needs booze 
Original summary: as good as it gets 
Predicted summary:  delicious


Review: things work well trouble leave one machine overnight sticks hard get otherwise great product 
Original summary: pretty cool 
Predicted summary:  great idea


Review: received product described minus one boxes received three four boxes cereal beware inept service 
Original summary: pack of four 
Predicted summary:  not what ordered


Review: love chili mix like another reviewer said earlier use little half chili powder packet provided also use rotel instead tomato sauce water comes great give try 
Original summary: great chili mix 
Predicted summary:  great chili


Review: tablet like teaspoon sugar sweetness need sweeten gallon gallon something adding pellets way easier opening bunch little packets even spooning sweetener pour pellets bottle cap count need whatever reason well kool aid brand soft drink mix mix well wyler flavor aid tastes find grain pellets sweetens quart soft drink packet well really feel like still getting aftertaste try pellets two packets splenda always add either nectasweet splenda prefer sweeter adding directly already chilled beverages give pellets minute dissolve stir well 
Original summary: nectasweet grain sugar substitute pellets 
Predicted summary:  it is not just for me
