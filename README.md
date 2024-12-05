Seven qubit quantum Fourier transform    
=================================  
Musawwadah Mukhtar, PhD  
https://github.com/DrMukhtar  

This is an implementation of a well known quantum algorithm, quantum Fourier transform. This is the first example of my personal project *petitZooQ*, my humble collection of implemented quantum algorithms.    

Quantum Fourier transform (QFT) is one of essential building block of many other quantum algorithm, including the Shor algorithm known for efficient number factorization. It is a powerful algorithm because the performance scale as $O((log N)^2)$, exponential speed-up compared to $N log N$ of Fast Fourier transform; here the number of qubit required is $log N$.  

To my knowledge, factorizing number would require QFT with 8 qubits in the first register; with the second register, this requires 12 qubits in total. This has motivated me to test QFT with 3 qubits up 7 qubits using the available IBM quantum processors. For each case, I compare the output of the quantum processor with the simulation result and the analytical result. The Qiskit package used to run the quantum processor includes simulation. Besides, we can also derive the analytical result. However, it would be impractical to simulate more than 15 qubits using your laptop. I found the case of seven qubits is the limit of their technology; tested on November 2024.  

The notebook requires 7 seconds of QPU time, relatively small compared to the 10 minutes of free monthly quota.  

To give a positive outlook, I believe the quantum processor performance will improve. Hopefully, the provided notebook in this project would help you aware of the state of the art of quantum computing.     

Here, you'll find the jupyter notebook. It's self-contained.    
However, to be able to reproduce the result, you have to install qiskit and have an account to access the IBM quantum processors. Indeed you have to get a token available in you account dashboard.   

To install Qiskit:  
https://docs.quantum.ibm.com/guides/install-qiskit

With your token, you should be able to run the notebook.  
I would like to point out the prompt to launch the notebook  
`
jupyter notebook path/to/notebook/7qubit_QFT.ipynb
`

I'll try to respond if you have any difficulty to reproduce the result.  
