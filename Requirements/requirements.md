# AML Use Case for Blockchain



## General Workflow

1. Client initiates an onboarding request to a member of the consortium.
2. Client is provided access to the consortium portal.
3. Client answers all of the required questions and provides the necessary documentation to satisfy the Client Due Diligence, KYC and AML data requirements. 

The data is stored directly on chain or on the IPFS, with a link back to the chain entry. 
4. Once Client has completed the data gathering, a request for validation is performed by the consortium.
5. Smart contracts will be executed to validate some or all of the data. 
6. The results will be published back to the client (and to member firms) based on the result of the smart contracts. 
7. 

## Product Backlog Items

1. Smart contract to automate expiry of client record based on risk rating. 
2. Integration with IPFS to store relevant client documents
3. User interface for entering the data that gets added to the blockchain
4. Privacy of client files must be maintained to any entity that is not part of the consortium
5. Smart contract to change risk rating based on PEP events.
6. Smart contract to change risk rating based on change in client jurisdiction.
7. Smart contract to change risk rating based on change in Beneficial Ownership. 
8. 

## Questions/Issues

1. How do we deal with data discrepancies for a client that has been onboarded to more than one member of the consortium?
2. How does the consortium make decisions on the data? For instance, what  allowable values would be in the schema.
3. How does the consortium come to consensus on validating the data provided by the client?
4. How will the data get in to the blockchain? Will we have a front end UI for users to interface with?