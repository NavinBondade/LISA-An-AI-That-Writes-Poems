# Writing Creative Poems With Deep Learning And NLP
<p align="center">
<a href="https://nbviewer.jupyter.org/github/NavinBondade/Lisa-An-AI-That-Writes-Lovely-Poems/blob/main/Notebook/Poem_Writing_AI%20%282%29.ipynb" target="_blank">
  <img align="center"  src="https://github.com/NavinBondade/Distinguishing-Fake-And-Real-News-With-Deep-Learning/blob/main/Graphs/button_if-github-fails-to-load-the-notebook-click-here%20(4).png?raw=true"/>
</a>
</p>
<img src="https://compote.slate.com/images/90194c2c-a99e-4c6f-9615-d9df031b6586.jpg" width="950" height="650">
<p>“There is no rule on how to write. Sometimes it comes easily and perfectly: sometimes it’s like drilling rock and then blasting it out with charges” — Ernest Hemingway</p></p>In line with Ernest Hemingway's observation that writing can either flow smoothly or require immense effort, this project harnesses the power of Natural Language Processing (NLP) and Deep Learning to craft beautiful poems with precision and creativity. The system combines the elegance of human language with advanced neural network architectures, designed to understand linguistic patterns, structures, and emotions. By leveraging large-scale data and modern machine learning algorithms, it generates poetry that is both emotionally resonant and technically refined, embodying the art of writing while reducing the cognitive strain associated with it. This system not only automates the creative process but also captures the nuances of poetic expression, offering a seamless fusion of technology and artistry.
</p>
<h2>Libraries Used</h2>
<ul>
  <li>Tensorflow</li>
  <li>Keras</li>
  <li>Numpy</li>
  <li>Pandas </li>
  <li>Matplotlib</li>
  <li>Seaborn</li>
  <li>Sklearn</li>
  <li>Spacy</li>
  <li>BeautifulSoup</li>
  <li>Wordcloud</li>
</ul>
<h2>Model Details</h2>
<p align="center">
<img src="https://github.com/NavinBondade/Lisa-An-AI-That-Writes-Lovely-Poems/blob/main/Graphs/Model.png" alt="model" >
</p> 
<p>For generating poetry, I have developed a sophisticated deep learning model that leverages the power of Long Short-Term Memory (LSTM) layers, which are particularly effective in capturing and retaining long-term dependencies within sequences of text. This is crucial for poetry generation, as it enables the model to understand and preserve the flow and meaning across different sentences or lines of a poem.

The architecture begins with an Embedding layer, which converts the input data into a dense representation, transforming words or tokens into vectors that can be more easily understood by the model. Following this, two LSTM layers are used sequentially. The first LSTM layer outputs a vector of size 100 from an input of 50 dimensions, capturing the contextual relationships between words in the sequence. The second LSTM further refines this representation, enabling the model to learn deeper patterns and dependencies.

After the LSTM layers, the architecture incorporates two Dense layers. The first Dense layer, using the ReLU (Rectified Linear Unit) activation function, helps in learning non-linear relationships, introducing complexity and ensuring that the model can handle intricate patterns in poetic structure. Batch Normalization is applied next, which normalizes the output from the Dense layer, improving the model’s learning efficiency and stability. Finally, the last Dense layer utilizes a softmax activation function, providing a probability distribution over the output space, which is crucial for selecting the next word or token in the poem.

This carefully designed architecture allows the model to balance creativity with structure, generating poems that are not only aesthetically pleasing but also coherent and contextually meaningful.</p>
<h2>Model Traning</h2>
<p>The model has trained for 170 epochs. During training, the model uses Adam as an optimizer and uses categorical cross-entropy as the loss function to penalize the model more when it makes a false prediction.</p>
<h2>Model Analysis</h2>
<p align="center">
<img src="https://github.com/NavinBondade/Lisa-An-AI-That-Writes-Lovely-Poems/blob/main/Graphs/Loss.png" alt="Loss" >
</p>
<p align="center">
<img src="https://github.com/NavinBondade/Lisa-An-AI-That-Writes-Lovely-Poems/blob/main/Graphs/Accuracy.png" alt="Accuracy" >
</p>
<p>After model training for 170 epochs, the model has achieved an impressive accuracy of 95% and a very low loss of 0.1782.</p>
<h2>Beautiful Poems (Model's Ouput)</h2>
<h3>Title: Friendship</h3>
<p>an worry as we send instead of my purpose an <br>
irish trunk tshirts when my hand back i found my <br>
cousin milton worked for a cable company the boy i <br>
have become the person who says darling who says sugarpie <br>
metaphor maybe nothing to do but brush back the tears</p>
<h3>Title: Love</h3>
<p>of us bear that have so near his message is <br>
anything central orchards flung out on the land urban forests <br>
or whose hollows was mean visited up there still sister <br>
and you are both let me be no one and <br>
yesterday something shattering happened not yesterday but several that is <br>
anything central orchards flung out on the land urban forests</p>
<h3>Title: Life</h3>
<p>passes through places pj duffy landscapes of south ulster patrick <br>
amount soul lady certainly for night give well historical the <br>
cat has the chance to make the sunlight beautiful to <br>
imagine the next weeping of the next ear you see <br>
everything looped spiraled circular thought but the labyrinths not a</p>
<h3>Title: Sadness</h3>
<p>i believe for love my own name love and warn <br>
of time and even whatever i know an grant you <br>
are running away from everyone who loves you from your <br>
husband is stretched out on the ground as if he <br>
brings me chocolate from the pentagon dark chocolates shaped like</p>

<h2>Conclusion</h2>
<p>In this project, I have created a deep learning model that foretells how the stock price of a company will behave by considering major news headlines with an impressive accuracy of 98 percent.</p>
