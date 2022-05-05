# PoeTree

Generate tree from poems or any texts.

Repository for [this google colab notebook]
(https://colab.research.google.com/drive/1kiyZIZuOYF35DyVN0QpTn8u0XDOFk0lU?usp=sharing)

## Desciption
This is a project that aimes to capture the poetic language and use it as source to generate poetic visuals, as well as giving the audiecne an insight into the shape and form of poetry with a graphical representation. I wish to create a intuitive connection between words and visuals, so that the audience can compare and contrast different poems by comparing their graphical forms.
<br/>

## Results
![at sunset](https://user-images.githubusercontent.com/73414720/166861264-f7b9fc44-fae8-4e7e-b7a1-b1646f59d03d.png)
![earth day](https://user-images.githubusercontent.com/73414720/166861273-a25db418-db58-4eed-be6b-0d94d793fdba.png)
![often i am permitted to return to a meadow](https://user-images.githubusercontent.com/73414720/166861280-0a188a67-dfe9-49a2-9d8d-642eeccdc264.png)
![rain](https://user-images.githubusercontent.com/73414720/166861283-31215ae9-f580-4da8-8968-82e095482f43.png)
![some feel rain](https://user-images.githubusercontent.com/73414720/166861289-0a650c33-721a-47d2-abad-b19deb34cb67.png)
![thank you](https://user-images.githubusercontent.com/73414720/166861295-6991f398-5c16-4944-8089-0b773d1d0555.png)
![the end of landscape](https://user-images.githubusercontent.com/73414720/166861300-d72ab2a5-dcb5-4a13-a49a-2bef1dcd5027.png)
![the seder's order](https://user-images.githubusercontent.com/73414720/166861313-58a58ee7-b652-4cfd-ab94-4f22e535adc0.png)
![the visiting hour](https://user-images.githubusercontent.com/73414720/166861318-b20f8142-2cd0-4cb5-ad59-8a8cbdd09200.png)
![tuesday, canal street](https://user-images.githubusercontent.com/73414720/166861327-1e0c3814-6922-4c77-8071-defef08828fe.png)
![work of love](https://user-images.githubusercontent.com/73414720/166861329-f35e5e6b-83a6-4ac3-af3d-2b2b04790445.png)
![did it hurt when you fell from heaven](https://user-images.githubusercontent.com/73414720/166861336-5755df5c-1a1a-4047-869c-3c75bc42cf38.png)
<br/>

## How it works
A single tree graph is gererated from each sentence in the input poem, with each vertical branch representing one semantic element (Most of the time, a word or a punctuation, but sometime a part of a word like "not" in cannot or "'s" in Monday's.). The tree's stucture is based on the sematic dependency tree of the sentense.  The color of the branch is based on the part-of-speech analysis of the semantic element, such maroon for verbs and deep green for nouns. The horizontal postion of each branch matches the postion of the word in the sentence when typed out and centered, as shown below.<br/>
![line 17](https://user-images.githubusercontent.com/73414720/166862078-50671d55-4004-40ab-9f86-39cbd9e4c984.png)
![line 9](https://user-images.githubusercontent.com/73414720/166862087-93e21af9-cb4b-4876-9ff8-46bd212cc02e.png)
![line 4](https://user-images.githubusercontent.com/73414720/166862102-692e81a3-777d-4f77-9cc6-8b82305fa195.png)
![line 16](https://user-images.githubusercontent.com/73414720/166862136-1a33abd4-acea-45be-b5de-4417716bcb58.png)
![line 12](https://user-images.githubusercontent.com/73414720/166862361-1f766717-8b22-4068-84dd-20de647b8b26.png)

Then these graphs are overlapped on top of each other, forming the final tree graph of the poem.
The poem is then typed out with the same coloration rule, next to the tree graph.<br/>
![Wide](https://user-images.githubusercontent.com/73414720/166862280-6f415a7b-5113-4245-b3a7-3ce117b7c3b4.png)
<br/>
## References and Credits
This project is using the following libraries:<br/>
[spaCy](https://spacy.io/): a NLP library and language model in python<br/>
[qahirah](https://github.com/ldo/qahirah): a python for [Cairo graphic library](https://www.cairographics.org/)<br/><br/>
Some of the poems enlisted in the examples are accessed from [Poetry Foundation website](https://www.poetryfoundation.org/), the rest are written by me.<br/>

