```mermaid

flowchart TB
subgraph one
direction TB
A-->B
B-->C
C-->D
D-->E
E-->F
F-->G
end
subgraph MakeWavFromInt
direction TB 
H-->I
I-->J
J-->K
K-->L
L-->M
M-->N
end

subgraph Main Function
direction TB 
O(Start)-->P
P["Set sample_rate
Set duration
Set n_samples
Set frequency
Set volume"
]-->Q
Q[Build a vector]-->RR
RR[set i to 0]-->R
R{"does i equal
number of samples?"
}--|"Yes
Pass vector into the make wav function"|-->S
R--|No|-->SS
SS["push new value onto vector"]-->R
S[[MakeWavFromInt]]-->T(End)
end

subgraph topfile
direction TB 
V(Start)-->W[Load Libraries]
W-->X[[Main Function]]
X-->Y(End)
end
```
