# TODO 

[Immediate]
- Its currently considered that the last block isn't verified 
fix: create a new dummy block as the latest block [ or look for the way that is used in practise ]

## Phase - 1 
- [x] Block Structure with   
      - student ID   
      - semester,subjects & marks  
      - Timestamp  
      - PreviousHash  
      - [x] immutability

- [x] SHA-256 hash chaining   
      - [x] Chain verification   
      - [x] Block verification  

- [x] Digital Signatures

- [x] CLI+TUI to
      - [x] Add a new block   
      - [x] Display chain
      - [x] Verify digital signature
      - [x] verify chain integrity  

- [ ] Json file storage  [ store hashes as well - 2 step verification (this and the verificatoin using ```prev_hash``` ) ]  


## Phase - 2 

- [ ] Complete TUI implementation

- [ ] Merkle Tree  
      - [ ] Hash subject-mark pair  
      - [ ] Store merkle root in block   
      - [ ] Support merkle proof generation and verification   
      
- [ ] Tamper Detection   
      - [ ] Validate full chain + merkle integrity  
      - [ ] CLI to check student's markscard integrity  

- [ ] ZKP-like logic (simulated)  
      - [ ] GPA > X show proof without revealing all marks   
      - [ ] Use selective disclose or dummy logic   

- [ ] GUI (Tkinter) or web(Flask) frontend (if time permits)   

- [ ] User restrictive priveleges - the data nor the hash should be modified . [ at certain intervals the hash of the blocks should be updated and verified. ]  


## Deliverables 

- [ ] code 
- [ ] CLI or GUI app  
- [ ] sample data (demo markscard)  
- [ ] Screenshots + README  
- [ ] Short report (explain structure + feature)  

## Experimental 

- [ ] consensus  [ multiple chains]  
- [ ] See if you can generate the hash for the whole data structure of the block instead of using another instance of *character*  
      - reduces code complexity    
      - increase code readability  

## Documentation
1. You'd should always read code and understand - that is the main reason behind existence of **COMMENTS**
2. Make sure to generate your private and public keys for digital signature and name them as ```private.pem``` and ```public.pem```
3. Remind me to create a makefile [here](instagram.com/ksurajsingh_13)
