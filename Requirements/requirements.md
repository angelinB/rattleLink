# AML Use Case for Blockchain



## New Client Onboarding Workflow

1. Client initiates an onboarding request to a member of the consortium.
2. Either the client is provided access to the consortium portal or the member firm uses the portal to enter the client data.
3. Client answers all of the required questions and provides the necessary documentation to satisfy the Client Due Diligence, KYC and AML data requirements. The data, forms and documents are stored to the IPFS, while a hash of the data and the CID is added to the block on the AML chain. 
4. Once Client has completed the data gathering, a request for validation is performed by the consortium.
5. Smart contracts will be executed to validate some or all of the data using external data sources e.g. Lexus Nexus, GLEIF, etc. 
6. The results, including the Client Risk Rating and other key information is added to the AML chain and is readable by all those that have been granted read access. 

## Maintenance Workflow - New PEP

1. A new Politically Exposed Person (PEP) has been identified through an external mechanism that has yet to be built. This triggers a workflow to be executed against the AML chain. 
2. A smart contract is executed to scan the Client entities in the AML chain to identify entities with a Board or Executive Officer with the same name as the new PEP. 
3. A case is opened in the portal for a member firm to adjudicate the change. The member firm that picks up the case is awarded the transaction fee for adjuticating the change. 
4. Once adjudicated, the member firm commits the change back to the chain. 
5. The smart contract is then executed to recalculate the risk rating and other attributes of each entity that has the PEP as either an Executive or Board member. These results are then updated on the AML chain.

## Product Backlog Items

1. Smart contract to automate expiry of client record based on risk rating. 
2. Integration with IPFS to store relevant client documents
3. User interface for entering the data that gets added to the blockchain
4. Privacy of client files must be maintained to any entity that is not part of the consortium
5. Smart contract to change risk rating based on PEP events.
6. Smart contract to change risk rating based on change in client jurisdiction.
7. Smart contract to change risk rating based on change in Beneficial Ownership. 


## Questions/Issues

1. How do we deal with data discrepancies for a client that has been onboarded to more than one member of the consortium?
2. How does the consortium make decisions on the data? For instance, what  allowable values would be in the schema.
3. How does the consortium come to consensus on validating the data provided by the client?
4. How will the data get in to the blockchain? Will we have a front end UI for users to interface with?