# AI Winter or AI Spring – where are we headed?

Any discussion on AI, today, invokes a host of emotions ranging from fear to anxiety to cheer! Here, I will try to paint a realistic picture of AI, covering its historical background, evolution and current state and debunk a few myths along the way.

## Is AI = ML = DL?
In order to answer that question, it’s imperative that we first look at the evolution of AI.

The field’s official founding can be traced back to a small workshop organised at Dartmouth college in 1956, by a young mathematician - John McCarthy. He had this idea of creating a ‘thinking machine’ which was shared by a few others, notably, Kevin Minsky, Herbert Simon, and Alan Newell, and they are collectively considered to be the founding fathers of AI.

But, what is this idea of a fully intelligent machine? And what do we really mean by artificial intelligence?

Unfortunately, ‘intelligence’, which is the central notion here, itself is somewhat ill-defined. Intelligence is sometimes binary - something is either intelligent or not. Sometimes, it is real-valued (continuous) - something is more intelligent than something else. And sometimes it is multi-dimensional - emotional, verbal, spatial, logical, artistic, social, etc. This lack of clear definition of intelligence carries over to the exact definition of artificial intelligence as well. However, it is broadly acknowledged that the original goal of AI was to build a machine that is no less intelligent than a human - in all aspects of intelligence, including - thinking, cognition, emotions, consciousness and others.

In the Dartmouth workshop, different participants had different opinions on the right way to approach AI.
* mathematicians promoted mathematical logic and deductive reasoning as the formalism to approach AI;
* Statisticians approached it from ‘data’ and promoted statistics and probability-based inductive methods - capturing any inherent uncertainty;
* Others took inspiration from neuro-science and psychology in suggesting to create brain-like programs

![](/images/venn.png){:style="float: right;margin-right: 7px;margin-top: 7px;"} These different approaches to AI broadly align with the three fields that emerged - logic-based (rule-based) AI, machine learning, and deep learning. The first one is also called symbolic AI and the latter two, sub-symbolic AI.

Over the last decade or so, deep learning has become predominant - so much so, that AI has become synonymous with deep learning! This is, however, a myth, an inaccuracy perpetuated by popular media. AI is a battery of different approaches and deep leaning is just one such approach. 

## Symbolic and sub-symbolic AI
Symbolic AI uses a vocabulary of symbols (words/phrases) along with rules to combine or process these symbols. The rules encode the constraints of the task. These systems can be engineered by humans, be imbued with human knowledge, and use human-understandable reasoning to solve problems. The proponents of symbolic AI believed that general intelligence can be captured entirely by such symbol-based programs. This dominated the AI field for initial decades and led to the development of several ‘expert systems’ that became popular then spanning application fields like medical diagnosis and legal decision making. One such expert system was MYCIN, developed in the 1970s to help physicians diagnose and treat blood diseases. This system comprised over 600 rules meticulously curated from interviews with several expert physicians.

Humans are adept at what has often been referred to as ‘fast perception’ - we can recognise faces, understand spoken words. How do we do that? This is often not something that we do consciously but happens sub-consciously. Sub-symbolic AI takes inspiration from neuroscience and seeks to capture these subconscious thought processes underlying fast perception. This field evolved from trying to model the human brain structure. One of the earliest sub symbolic models was the ‘perceptron’ model by Frank Rosenblatt in the late 1950s.

![](/images/nn.png)

Perceptrons are inspired by the way in which neurons process information. A neuron receives input from other neurons that connect to it. And roughly speaking, what’s happening is that the neuron sums up all the input it receives and if the sum crosses certain threshold, then it fires. These synapses, connections between neurons, have different strengths. Neuroscientists believe that adjustments to the strengths of these connections between neurons is how learning takes place in the brain. Rosenblatt’s perceptron mimics this information processing of neurons. Rosenblatt showed that given the right set of weights, a perceptron can work quite well on perceptual tasks like object detection. In order to learn these weights, Rosenblatt came up with the “perceptron learning algorithm” which falls under the class of supervised learning algorithms in AI.

The advocates of sub-symbolic AI believe that language-specific symbols (and operators) that underlie symbolic AI approaches are hard to define and cannot achieve general purpose AI - rather these should emerge from neural-like architectures. These initial developments led to a lot of excitement among practitioners of sub-symbolic AI.

But this was short-lived as several limitations of perceptrons surfaced. Minsky and Papert showed that perceptrons are suitable for a narrow class of problems. In order for them to be applicable to practical perceptual tasks would require multiple layers of these networks (referred to as Multi-layer Perceptrons or MLPs in short) and perceptron learning algorithm could not scale to learning large number of weights across multiple layers.

As a result, sub-symbolic AI fell off the radar. By the mid-1980s, symbolic AI approaches that rely on humans to create rules were also increasingly revealing themselves to be brittle – error-prone and often unable to generalize. It became increasingly evident that, the original goals of AI—computers that could converse with us in natural language, describe what they saw through their camera eyes, learn new concepts after seeing only a few examples—are things that young children can easily do, but, surprisingly, are harder for AI to achieve.

### AI winter set in.

### But haven’t we now solved these “hard for AI” problems now?

Last couple of decades has seen a resurgence of the field of AI. If there’s one incident that changed the practical perception of AI was that of deep blue beating the chess champion Garry Kasparov back in the late 1990s! By mid-2000s, AI started becoming more pervasive. Google translate, self-driving cars, virtual assistants like Apple Siri, Amazon Alexa, automated video subtitles, Facebook’s face recognition, Flikr’s automatic labelling of photos, are all well known to us. Other incidents that took the world by storm, more recently, were IBM Watson defeating human champions in the game of Jeopardy and AlphaGo defeating the human Go champion. On the task of automatic speech recognition, AI researchers from Google have achieved a word-error-rate (WER) of 4.7% - at par with human transcriptionists! Image classification error rate has dropped to around 3.1% on the ImageNet dataset!

### We are living in an AI spring. What is driving this resurgence?

Deep learning! Think of it as multi-layer perceptrons (MLPs) on steroids. Sub-symbolic AI is back with a bang and is spurred by three key developments – 
1. development of sophisticated statistical and optimization techniques, notably, the back propagation algorithm – an algorithm for learning large scale multi-layer perceptrons;
1. availability of massive amounts of data and ability to label data through crowd sourcing tools like Amazon’s Mechanical Turk;
1. increased computational power made possible due to leveraging GPU-based technology and libraries for training large scale deep learning models.

## So has AI arrived then?

On one hand, there is a feeling of excitement surrounding these achievements of AI that seem to suggest that we have reached human-level intelligence. On the other hand, this is shrouded by a feeling of anxiety and fear – think about your favourite doomsday scenario (“will AI take my job?”, “singularity!”).

What is required, though, is a careful scientific characterisation of the current AI developments and their potential reach. Lack of that is the reason behind current misconceptions surrounding AI progress and where it may lead us, leaving a lot to the imagination.

Remember, the original goal of AI was to develop an automated system, as much or more intelligent than humans!

What we have managed to achieve though is:
* an improved ability to fit functions to data, through availability of massive amounts of data, increased computational power and sophisticated statistical and optimization techniques;
* a class of narrow applications that allow for compact representations (functions) and can be efficiently evaluated without requiring reasoning;
* a departure from original objectives and measures of success that have reduced the technical challenges while maintaining our ability to capitalise on the obtained results commercially.

Bottomline is that we are still far from capturing the human intelligence.

How far you ask? I will not answer that, but, instead, raise these provocations – 

1. Has AI surpassed humans at object recognition? This conclusion is riddled with several caveats. Firstly, this is on a specific dataset – ImageNet and in fact, these models do not perform as well in recognizing objects in images in the wild. Secondly, this is on the top-5 accuracy metric, a relaxation of the stricter top-1 metric. And thirdly, the reference to “humans”, here, is inaccurate, as the experiment involved a single human – a scientist by the name Andrej Karpathy. So, this claim needs to be taken with a large grain of salt!
1. Dog or a Frisbee? When a human says that a photo contains, say, a dog, we assume it’s because the human actually saw a dog in the photo. But if a deep learning model correctly says “dog,” it could be basing this classification on something else in the image—a tennis ball, a Frisbee, a chewed-up shoe—that was often associated with dogs in the training images. These kinds of correlations have often ended up fooling machines!
1. Does human brain learn via backpropagation? Humans often learn an open-ended set of categories, require only a few examples, they ask questions, infer abstractions and connections between concepts. Most successful deep learning models, on the other hand, require supervision from large amounts of labeled training data. Supervised learning is not a viable path to general-purpose AI!
1. What is the network learning? Models learn what they observe in the data rather than what we want them to learn. For instance, addition of white noise to an image causes an image classification model to misclassify, although, the resulting image “looks” like the original one. Superficial changes to images can trick deep learning models! 
1. The problem of bias! Errors due to racial or gender biases have been noted frequently in vision systems powered by deep learning. For instance, in pictures of men standing in the kitchen, an image classification model classifies “men” as “women”. These biased models can often lead to damaging consequences.

In summary, while much of the optimism surrounding AI is based on the recent successes of deep learning, these programs are still examples of what is called “narrow” or “weak” AI. This is not in any derogatory sense but just an acknowledgement of the fact that these systems can perform only a narrowly defined task. This is in contrast to strong or general AI - the kind that is portrayed in movies - that can do almost everything that a human can do and more! General AI might have been the original goal of the field, but achieving it has certainly turned out to be much harder than expected.

