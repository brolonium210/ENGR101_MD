```mermaid
        graph

    subgraph Generate Waveform
        direction TB
        BJ[[Generate Waveform]] --> BK[Loop through each sample]
        BK --> BL[Calculate time between samples]
        BL --> BM[Calculate current value]
        BM --> BN[Add value to waveform vector]
        BN --> BO{"Have we reached 
        number of samples?"}
        BO -->|Yes| BP[Exit Function]
        BO -->|No| BK
    end

    subgraph Main
        direction TB
        A[Main] --> B["Include iostream ,math.h,vector and wav.hpp"]
        B --> C[Call Main]
        C -->D["Set sample rate to 44100
        Set duration to 5 seconds
        Calculate number of samples
        Set freq to 300 Hz
        Set volume(Amplitude)"]
    D --> G[Create empty vector for waveform]
    G --> J[[Generate Waveform]]
    J --> R[Call MakeWavFromVector with parameters]
    R --> S[Clear waveform vector]
    S --> T[End Main]
    end
```
Include Libraries

Define Main
        Set sample rate to 44100
        Set duration to 5 seconds
        Set number of samples to sample rate * duration
        Set freq to 300 Hz
        Set volume(Amplitude)
        Create an empty vector for waveform

Generate Waveform
        for every sample from 0 to number of samples:
            recalculate the position on the wave(dt) as the current sample index divided by the total number of samples.
                then Calculate the waveform value for the current sample as volume multiplied by the sine of 2π times the frequency times dt.
                    then Push this value to the waveform vector
        
When Generate has finished
        Call MakeWavFromVector from the wav.hpp 
            then pass the arguments of filename "toneCore01.wav" ,total number of samples and waveform vector.
        Clear the waveform vector to free up memory.
        Return 0 to indicate successful completion.
