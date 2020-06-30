Add ADFS Relying Party Trust
===

1. On your ADFS server, open the ADFS Management console(mmc), expand **Trust Relationships** and select the **Relying Party Trusts** node. In the **Actions** pane, click **Add Relying Party Trust**
![](https://i.imgur.com/0CcxB2m.png)

2. Click **Start** then paste the **Entity ID** url in to the **Federation Metadata** address field and click **Next**.
Entity ID: https://ns1.asuscomm.com/simplesaml/module.php/saml/sp/metadata.php/default-sp
![](https://i.imgur.com/F5gOGaT.png)

3. Accept the warning.
![](https://i.imgur.com/hBjwh2x.png)

4. Reach the **Ready To Add Trust** page.check the **Encryption** and **Signature** tabs
![](https://i.imgur.com/StB8VKN.png)

5. Click **Next** and check the **ns1.asuscomm.com** Relying Party Trust is added.

6. Select the **ns1.asuscomm.com** and then click **Edit Claim Rules…**
![](https://i.imgur.com/4eJeeIR.png)

7. Add an **Issuance Transform Rule** based on the **Send LDAP Attributes as Claims** template. 
![](https://i.imgur.com/DOtjT5L.png)

8. Add another Issuance Transform Rule but this time based on the **Transform an Incoming Claim** template.
![](https://i.imgur.com/INAr7jo.png)

9. Once configured, you should have two Issuance Transform Rules that look as follows:
![](https://i.imgur.com/MYq7egF.png)

