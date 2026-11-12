# CKBuilder

Dev log for the Nervos CKBuilder program. Weekly reports, notes and code from working through the CKBuilder handbook go here.

## Onboarding

- **2026-11-09:** Got OffCKB 0.4.13 running a local devnet (CKB 0.208.0). Deployed the hello-world contract from the TypeScript template. The deploy tx `0x717f98eb...ae974` was committed in block 12.

![OffCKB devnet deploy](images/offckb-deploy-proof.png)

## Week 1: OffCKB and the hello-world contract

9 to 12 November 2026. AI assisted with this report and ran the lab on 12 November. The personal reflection below was confirmed by the participant and translated into English with AI assistance.

The hello-world contract from the TypeScript template was deployed to the local OffCKB devnet on 9 November. The saved deployment output records a committed transaction, and the screenshot shows it in block 12.

On 12 November, an automated lab run confirmed that the contract's code cell was still live. It contained 1,305 bytes of compiled code and had a capacity of 1,366 CKB. Its data hash matched the code hash in the deployment configuration.

The devnet test passed, and its transaction was committed. The output used the CKB JavaScript VM to run hello-world as a type script. The node log included `hello-world script loaded`, confirming that the script executed. The transaction used 5,605,306 cycles across its lock and type scripts.

The manual exercise that changes `return 0` to `return 1` has not been completed. That exercise checks how a script rejects a transaction.

### Personal reflection

I know the transaction was confirmed, but I still don't understand all the fields in the RPC response.

### Evidence

These transaction hashes belong to the local devnet.

1. Deployment: `0x717f98ebdc961a4a5daa2cdbff938c38a5e39f2260c73ba36f738c56916ae974`.
2. Lab transaction: `0x541f3f2b8580f9466e10b11f2f60686203a94455659b699faa5acb4306f931ab`.
3. [Lab output from 12 November](evidence/week-1-lab.log).

![Deployment evidence captured on 9 November](images/offckb-deploy-proof.png)
