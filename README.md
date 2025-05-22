# JSON-policy-in-Azure
This JSON code will block any VM creation otuside the specified location in the code
I created this policy is azure portal. I wanted to test some things I learned online and what better way to do so than putting my knowledge to the test.

What I did:
- In my Azure Portla I went to Azure Policy
- Under "Authoring" on the left pane, I clicked "Dedinitions"
- Clicked "Policy Definitions"
- Defined the location, which in my case is my subscription, meaning no matter the resource group as long as it's under the same subscription the policy of denying VMs outside the allowed location will apply
- Defined a name for my policy
- Under "Category" clicked "Create new", then enter the name of the category
- In the template JSON file paste the code I provided and click "Save"
- A new page will open at the top right click "Assign policy"
- Double check the configuration and make sure everything seems OK
- Click "Review + Create". The new policy will take effect within 5 to 15 minutes.
