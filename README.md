# Building Hadoop Application
 
## Hadoop WordCount operation occurs in 3 stages 
1. Mapper Phase 
2. Shuffle Phase 
3. Reducer Phase

## Hadoop WordCount Example- Mapper Phase Execution
The text from the input text file is tokenized into words to form a key value pair with all the words present in the 
input text file. The key is the word from the input file and value is ‗1‘. 

For instance if you consider the sentence ―An elephant is an animal‖. The mapper phase in the WordCount example 
will split the string into individual tokens i.e. words. In this case, the entire sentence will be split into 5 tokens (one 
for each word) with a value 1 as shown below –
Key-Value pairs from Hadoop Map Phase Execution

(an,1) 

(elephant,1) 

(is,1) 

(an,1) 

(animal,1) 

If you would like more information about Big Data and Hadoop Certification, please click the orange "Request Info" 
button on top of this page. 

## Hadoop WordCount Example- Shuffle Phase Execution 
After the map phase execution is completed successfully, shuffle phase is executed automatically wherein the keyvalue pairs generated in the map phase are taken as input and then sorted in alphabetical order. After the shuffle 
phase is executed from the WordCount example code, the output will look like this

(an,1) 

(an,1) 

(animal,1) 

(elephant,1) 

(is,1) 
