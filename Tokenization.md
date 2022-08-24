# **TOKENIZATION**

The tokenization process (PR2) illustrates how different functions are activated to generate the required smart contracts to tokenize the creator’s OSS-projects and start receiving funds through stakes.social, a decentralized crowdfunding platform.

After the onboarding process (PR1), the creator’s personal information and tokenization credentials are at stakes.social backend, a virtual machine. it will use the creator’s identity with their OSS-project when the create function of the tokenization engine is run.

Then, the program will create a smart property contract, which links the creator with the asset. By default, ten million property tokens are created as a total supply representing the assets’ ownership. 5% of that supply (500,000 tokens) will be allocated to a treasury contract between the creator and Dev Null AG, the legal entity of Dev Protocol, as a fee for the service. The treasury contract is owned by Dev Protocol. The creator will hold the rest (9,500,000 tokens) to own and use as they see fit.

After that, the tokenization engine will sign up the creator to “Khaos”, an oracle service designed to bring Internet data into blockchains. In this activity, “Khaos” server will prepare the assets to be authenticated through an API with the asset’s platform. There are two types of assets that creators can tokenize, GitHub repositories and Youtube content. Depending on the asset type, the “Khaos” authentication process may differ: 1) for GitHub repositories, the creator can log in to GitHub and create a Personal Access Token (PAT) and sign in to the authenticated repository name with the private key of their wallet, 2) for Youtube, the creator sets an OAuth token, a protocol for authorizing access to personal user data, and sign in with the ID of the Youtube channel using the private key of the creator's wallet. The tokenization engine will take the latter credentials and run the “Khaos” signing API.

Once the above happens, the authentication function will run, verifying the asset´s ownership with the market contract, which was created and authenticated during the onboarding process (PR1). Finally, the property contract links with the market contract. If the creator has more property contracts to add, the process from the create function step to the link between property and market contract step will repeat.

If the already onboarded creator decides to tokenize another OSS-project. The onboarding process will repeat, which implies making a formal, content verification and market validation again. If the OSS project is approved, the creator will be able to repeat the tokenized activity. Additionally, the creator need to confirm that KYC-data is still up to date, otherwise, they need to be changed.