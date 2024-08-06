## We have taken a Shakespere data set which is of 1 MB and we train GPT model on this data to generate text which is similar to the input data file

### Here is the config that we have used for building the GPT

* batch_size = 16
* block_size = 256 (which is the context length)
* vocab_size = 65
* n_emb = 128
* num_heads = 6 
* n_layers = 6
* dropout = 0.0
* learning_rate = 1e-3 
* min_lr = learning_rate * 0.1 ( This is calculated because we have used Cosine LR scheduler )

### Additional Implementations which are inspired from Transformers, GPT2 & LLama Research Papers

* Weights are initialized with std == 0.02 and mean == 0
* AdamW optimizer with weight decay of 0.1 and betas (0.9,0.95) is used
* Normalized the Gradients in the Training loop 

### Sample Output from the Model

RICHMOND:
Hold received the grant are well caught her,
Side even chysel. Have wask me her one safe
Than I was acpin to your viols talk in
His upon you: I own mean bhild up awas than thee
are is of fak! my tongued and doings; for eath
of m
ion,
More to one so not lightly spirits,
But save appriof at officersation me
To swill givil out enter to the mileguable,
Being and to-night root aritoroous be thus
Time letters for him up to me a
For some left by of late him that took find appear,
Ere devi

Thou should I think what he asvices; therefore
To bear enmity, that to slow their do
that the bover of all-hood your limbs:
You wilt first.

ANGELO:
If my best, 'let y--


ISABELLA:
O the city; enough, look to hear shall be comes!--

BENVOLIO:
For Marcius:
ays to fine mad, sit by this ours.
To fleser, pardon, truspetitlut, the soon.

SICINIUS:
Now it is sow; since take you of thy mother's
With slain off, let I have drownrage, let you
do.

MENENIUS:
O--Mercy, if you,
Love's where to give me and me towards with
QUEEN MARGARET:
We will, it issue and it is their crown;
And and misselGuclary from a lady from well,
The clamortors, sake we fill me measure in wife.

QUEEN MARGARET:
Yea, no, what a marriage of my Gloucester
With a hrouble south to the pridence command;
H

#### Note: This Implementation work is done with help of Andrej Karpathy nanoGPT repo 
