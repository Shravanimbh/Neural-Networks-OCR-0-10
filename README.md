# Neural-Networks-OCR-0-10
This was a workshop under IEEE SIES GST , Focusing on understanding the core principles of Machine Learning.
Single Neuron Output :
neuron output=input⋅weight+bias
output=∑i=0n(inputi⋅weighti)+biases
Here input and weight are arrays of float values of which dot product is calculated.
ReLU is mostly used to activate hidden layers.
ReLU(x)=max(0,x)
SoftMax Activation
Softmax(zi)=ezi∑jezj
Loss Calculation (Categorical Cross-Entropy)
Loss=−∑iyilog(pi)
Adam Optimizer
Compute the biased first moment estimate  mt 
mt=β1⋅mt−1+(1−β1)⋅gt 
where  gt  is the gradient at time step  t .
Compute the biased second raw moment estimate  vt :
vt=β2⋅vt−1+(1−β2)⋅g2t 
Compute bias-corrected first moment estimate  m^t :
m^t=mt1−βt1 
Compute bias-corrected second raw moment estimate  v^t :
mt=β1⋅mt−1+(1−β1)⋅gt 
Update the parameters  θ :
θt=θt−1−α⋅v^tm^t−−−√+ϵ
