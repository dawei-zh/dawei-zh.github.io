---
permalink: /
title: "About Dawei Zhong"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Welcome to my homepage. My name is Dawei Zhong and I am a second year PhD student in the Department of Physics & Astronomy at University of Southern California. 

Here is a test for math equation display: 



In the noisy teleportation case, if Alice prepares $|\Phi^{+}\rangle$ and sends one share to Bob via dephasing channel $\mathcal{N}(\rho)$​, where


$$
\mathcal{N}(\rho) = (1-p)I\rho I + pZ\rho Z\tag{1}\label{1}
$$


then when Alice and Bob performs usual teleportation protocol, the joint state of system $A', A$ and $B$ becomes


$$
|\psi\rangle_{A'}\langle\psi|_{A'} \otimes (I_{A} \otimes \mathcal{N}_{B}) (|\Phi^{+}\rangle_{AB}\langle \Phi^{+}|_{AB})\tag{2}\label{2}
$$
From eq. $\eqref{1}$ we notice that $\mathcal{N}$ can be written in Kraus representation form, according to appendix, we can write the map $I_{A} \otimes \mathcal{N}_{B}$ as


$$
\begin{align}
(I_{A} \otimes \mathcal{N}_{B})(\rho) &= \sum_{\alpha}(I_{A}\otimes K_{B,\alpha})\rho (I_{A}\otimes K_{B,\alpha})^{\dagger} \\
&= (1-p)(I_{A}\otimes I_{B})\rho (I_{A}\otimes I_{B}) + p(I_{A}\otimes Z_{B})\rho (I_{A}\otimes Z_{B}) \\
&= (1-p)\rho  + p(I_{A}\otimes Z_{B})\rho (I_{A}\otimes Z_{B})
\end{align}\tag{3}\label{3}
$$


We can use eq. $\eqref{3}$ to re-write eq. $\eqref{2}$ as


$$
\begin{align}
|\psi\rangle_{A'}\langle\psi|_{A'} \otimes (I_{A} \otimes \mathcal{N}_{B}) (|\Phi^{+}\rangle_{AB}\langle \Phi^{+}|_{AB}) =& (1-p)|\psi\rangle_{A'}\langle\psi|_{A'} \otimes |\Phi^{+}\rangle_{AB}\langle \Phi^{+}|_{AB} \\
&+ p|\psi\rangle_{A'}\langle\psi|_{A'} \otimes (I_A\otimes Z_B)|\Phi^{+}\rangle_{AB}\langle \Phi^{+}|_{AB}(I_A\otimes Z_B) \\
=& (1-p)|\psi\rangle_{A'}\langle\psi|_{A'} \otimes |\Phi^{+}\rangle_{AB}\langle \Phi^{+}|_{AB} \\
&+ p|\psi\rangle_{A'}\langle\psi|_{A'} \otimes |\Phi^{-}\rangle_{AB}\langle \Phi^{-}|_{AB} \\
\end{align}\tag{4}\label{4}
$$


The first term of eq. $\eqref{4}$​​ is the noiseless teleportation, and we can write it in following way,


$$
|\psi\rangle_{A'}|\Phi^{+}\rangle_{AB}=  |\Phi^{+}\rangle_{A'A} |\psi\rangle_B + |\Phi^{-}\rangle_{A'A}Z|\psi\rangle_B +  |\Psi^{+}\rangle_{A'A}X|\psi\rangle_B + |\Psi^{-}\rangle_{A'A}XZ|\psi\rangle_{B}\tag{5}\label{5}
$$


For the second term of eq. $\eqref{4}$​​, we could follow the analysis of noiseless teleportation, and re-write the joint state in the following way, 
$$
\begin{align}
|\psi\rangle_{A'}|\Phi^{-}\rangle_{AB} =& (\alpha|0\rangle_{A'} + \beta|1\rangle_{A'}) \left(\frac{|00\rangle_{AB} - |11\rangle_{AB}}{\sqrt{2}}\right) \\
=& \frac{1}{\sqrt{2}}(\alpha|000\rangle_{A'AB} - \alpha|011\rangle_{A'AB} + \beta|100\rangle_{A'AB} - \beta|111\rangle_{A'AB})
\end{align}\tag{6}\label{6}
$$
Note that we can express two qubits state with Bell basis,
$$
\begin{align}
|00\rangle_{A'A} &= \frac{1}{\sqrt{2}}(|\Phi^{+}\rangle_{A'A} + |\Phi^{-}\rangle_{A'A}) \\
|01\rangle_{A'A} &= \frac{1}{\sqrt{2}}(|\Psi^{+}\rangle_{A'A} + |\Psi^{-}\rangle_{A'A}) \\
|10\rangle_{A'A} &= \frac{1}{\sqrt{2}}(|\Psi^{+}\rangle_{A'A} - |\Psi^{-}\rangle_{A'A}) \\
|11\rangle_{A'A} &= \frac{1}{\sqrt{2}}(|\Phi^{+}\rangle_{A'A} - |\Phi^{-}\rangle_{A'A}) \\
\end{align}\tag{7}\label{7}
$$
Substitute eq. $\eqref{7}$​ into eq. $\eqref{6}$​, we have
$$
\begin{align}
|\psi\rangle_{A'}|\Phi^{-}\rangle_{AB}=& \frac{1}{\sqrt{2}}(\alpha|000\rangle_{A'AB} - \alpha|011\rangle_{A'AB} + \beta|100\rangle_{A'AB} - \beta|111\rangle_{A'AB}) \\
=& \left[\alpha(|\Phi^{+}\rangle_{A'A} + |\Phi^{-}\rangle_{A'A}) |0\rangle_{B}
- \alpha(|\Psi^{+}\rangle_{A'A} + |\Psi^{-}\rangle_{A'A})|1\rangle_{B}\right. \\
&+ \left.\beta(|\Psi^{+}\rangle_{A'A} - |\Psi^{-}\rangle_{A'A})|0\rangle_{B} 
- \beta(|\Phi^{+}\rangle_{A'A} - |\Phi^{-}\rangle_{A'A})|1\rangle_{B}\right] \\
=& |\Phi^{+}\rangle_{A'A}(\alpha |0\rangle_{B}  - \beta|1\rangle_{B} ) + |\Phi^{-}\rangle_{A'A}(\alpha |0\rangle_{B}  + \beta|1\rangle_{B} ) \\
&-  |\Psi^{+}\rangle_{A'A}(\alpha |1\rangle_{B}  - \beta|0\rangle_{B} ) - |\Psi^{-}\rangle_{A'A}(\alpha |1\rangle_{B}  + \beta|0\rangle_{B} ) \\
=& |\Phi^{+}\rangle_{A'A} Z|\psi\rangle_B + |\Phi^{-}\rangle_{A'A}ZZ|\psi\rangle_B -  |\Psi^{+}\rangle_{A'A}XZ|\psi\rangle_B - |\Psi^{-}\rangle_{A'A}XZZ|\psi\rangle_{B}
\end{align}\tag{8}\label{8}
$$
From eq. $\eqref{4},\eqref{5}$ and eq. $\eqref{8}$, we know that after Alice measures $A'$ and $A$ and transmit two classcial bits to Bob for recovery, Bob will finally get a mixed state, 
$$
\rho_B = (1-p)|\psi\rangle_B\langle \psi|_B + p Z|\psi\rangle_B\langle \psi|_BZ\tag{9}
$$
which is equivalent as sending Bob $|\psi\rangle$ directly from the dephasing channel.



Kkk

# Others

During my academic career, especially at the early stage, I often find it hard to have high-quality, useful resource and I think this obstruct many passionate people to go deeper. Here I summarize some very useful information that would pave one's way on a well-equipped researcher in my industry. I include basic equation sheets, useful visualization tools, useful computer skills and everything maybe helpful. Please visit this and this for more details...(to be continued)

# Contact

Please send me a email via [daweiz@usc.edu](mailto:daweiz@usc.edu)
