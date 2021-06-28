# शासन और संचालन

25 अप्रैल, 2021 को [YIP-61: शासन 2.0](https://gov.yearn.finance/t/yip-61-governance-2-0/10460) पारित होने के बाद से, एयरन ने **मल्टी-डाओ** संक्रमण शुरू किया जो, **विवश प्रतिनिधिमंडल** द्वारा प्रबंधित है । यह दृष्टिकोण विकेंद्रीकरण के पर्याप्त स्तर को बनाए रखते हुए प्रोटोकॉल विकास को नौकरशाही द्वारा कठोर नहीं होने देता है।

मल्टी-डाओ  विकेंद्रीकृत स्वायत्त संगठनों (डाओ) की तरल संख्या को संदर्भित करता है जो प्रोटोकॉल में कुछ अनोखे तरीके से योगदान करते हैं। इन स्वतंत्र समूहों में YFI धारक, yTeams(व्ह्यटीमस) और Multisig (मल्टीसिग) शामिल हैं।

- **YFI धारक** प्रोटोकॉल या प्रोटोकॉल शासन संरचना में परिवर्तन के लिए वोट करते हैं
- **yTeams(व्ह्यटीमस)** प्रोटोकॉल या प्रासंगिक संचालन के विशिष्ट पहलुओं पर ध्यान केंद्रित करते हैं
- **Multisig(मल्टीसिग)** सदस्य किसी भी ऑन-चेन निर्णय को निष्पादित या प्रतिबंध करते हैं

टोकन धारकों का अंतिम अधिकार है, yTeams कि मौजूदगी पर,  मल्टीसिग कि हिस्सेदारी  पर, और प्रत्येक समूह के परिचालन नियंत्रण की सीमाओं पर। 'विवश प्रतिनिधिमंडल' इस शब्द की उत्पत्ति टोकन धारकों से हुई है जो विशिष्ट शक्तियों को विभिन्न समूहों को सौंपते हैं जो एयरन का निर्माण और प्रबंधन करते हैं।

शासन का एक आसान प्रवाह इस तरह दिखेगा:

    1. YFI धारक yTeams की सीमाएं बनाते हैं, उनको नष्ट करते हैं और उनकी परिभाषित करते हैं।
    2. yTeam निर्णय के बारे में yTx को सूचित करती है।
    3. yTx एक प्रत्यायोजित लेनदेन बनाता है और उसे मल्टीसिग को भेजता है।
    4. मल्टीसिग लेन-देन को निष्पादित या निषेध करता है।
    
## डाओ की  जिम्मेदारियां

![](https://i.imgur.com/IDysF5O.png)

### टोकन धारक 

यह [YFI टोकन](https://docs.yearn.finance/governance/yfi) धारक का कर्तव्य है कि वह प्रोटोकॉल में सुधार करने वाले प्रस्तावों को बनाएं और उनके लिए मतदान करें।

| प्रस्ताव | विवरण |
|-----------|--------------|
|एयरन सुधार प्रस्ताव (YIP)|YFI धारकों को प्रत्यायोजित किसी शक्ति पर या प्रगणित शक्तियों के दायरे से बाहर निष्पादित करने का प्रस्ताव||
|एयरन प्रतिनिधिमंडल प्रस्ताव (YDP)|जहां किसी भी असतत निर्णय लेने की शक्ति को प्रत्यायोजित किया जाता है, उसे बदलने का प्रस्ताव|
|एयरन संकेतन प्रस्ताव (YSP)|किसी भी मुद्दे पर सामुदायिक भावनाओं या मंशा को इंगित करने के लिए एक गैर-बाध्यकारी प्रस्ताव|

विशेष रूप से, ये प्रस्ताव टोकन धारकों को निम्नलिखित निर्णय लेने की अनुमति देते हैं: 

| शक्ति | विवरण |
|-------|-------------|
|शक्तियों का प्रबंधन करें|YFI धारक yTeams को या उससे असतत शक्तियाँ बनाने, बाटने   या रद्द करने के लिए मतदान कर सकते हैं|
|YFI टोकन का अनुबंध बदलें|YFI टोकन अनुबंध के साथ कोई भी बातचीत, जैसे कि YFI का टकसाल करना या टकसाल की चाबियों को बर्न करना, YFI धारकों के नियंत्रण में रहता है।|
|शुल्क निर्धारित करें|एयरन प्रोटोकॉल में मानक शुल्क संरचना निर्धारित करें|
|मल्टीसिग के हस्ताक्षरकर्ताओं को बदलें|चूंकि मल्टीसिग निकट अवधि में महत्वपूर्ण शक्तियों को जारी रखेगा, केवल YFI धारक ही अपने हस्ताक्षरकर्ताओं को बदलने के लिए मतदान कर सकते हैं|
|yTeams की पुष्टि करें|यह नियंत्रित करने के लिए कि कौन-सी yTeams प्रत्यायोजित शक्तियां धारण कर सकती हैं, औपचारिक रूप से yTeams की पुष्टि करें या उन्हें निष्क्रिय करें|
|yOps हस्ताक्षरकर्ता बदलें|चूंकि yOps के पास अन्य yTeams के हस्ताक्षरकर्ताओं को बदलने की शक्ति है, यह yOps के हस्ताक्षरकर्ताओं को बदलने की एक विशेष शक्ति है|
|राजकोष के धन खर्च करें|राजकोष से धन खर्च करें|
|YIP शक्ति |YFI धारकों के पास पहले से गैर प्रत्यायोजित किसी भी चीज़ पर YIP का प्रस्ताव करने की शक्ति है|
### yTeams

Each yTeam has an objective and discrete powers which are defined by token holders. They can be broken further into membership pools, which are separate groups of contributors working towards similar goals as the overarching team. Additionally, one membership pool can bet a part of multiple yTeams.

| yTeam | Objective | Membership Pool |
|-------|-----------|-----------------|
|yGuard|Protect the vaults|YFI Protocol Dev, YFI Strategists, YFI Mechanics, YFI Secret Admirers|
|yBrain|Manage the strats|YFI Strategists|
|yDev|Manage the protocol|YFI Protocol Dev|
|yPeople|Curate the team|YFI Compensation Working Group, YFI Advisors|
|yBudget|Spend money well|YFI Finances, YFI Advisors|
|yFarm|Grow the treasury|YFI Secret Admirers, YFI Secret Entrance|
|yTx|Write transactions|YFI Doers|
|yOps|Coordinate contributors|YFI Ops|

Each yTeam is assigned specific decision-making powers, defined by YIP-61: 

| yTeam | Power | Description |
|-------|-------|-------------|
|yGuard|Emergency Powers|Immediately intervene in case of attack or bug to shutdown or rollback strategies or vaults|
|yBrain|Manage Strategies|Activate, deactivate, tune, and maintain strategies|
|yDev|Define Yearn Protocol|Decide what code is considered part of yearn and what isn’t|
|yDev|Manage Protocol|Maintain and improve the Yearn Protocol|
|yDev|Add Strategies|Add new strategies to vaults|
|yTx|Delegate Transactions|Create delegated transactions for the multisig to sign and execute|
|yPeople|Pay Team|Create, deploy, modify, or terminate Yearn compensation packages|
|yBudget|Set Budgets|Create budgets for coordinape, grants, hiring, operations, or other workstreams|
|yFarm|Farm Treasury|Farm with the treasury and make decisions on airdrops|
|yOps|Ratify yTeam Signers|Formally approve or remove signers for each yTeam|

### Multisig 

Decisions issued by yTeams will be executed on-chain by the Multisig until a more decentralized system is approved for implimentation. In the mean time, the [Multisig](https://docs.yearn.finance/resources/faq#who-is-on-the-multisig) controls the following:


| Power | Description |
|-------|-------------|
|Execution Power|The power to execute decisions made by YFI holders and yTeams on-chain|
|Veto Power|This power allows the Multisig to veto any decision and ideally should not be needed|
|Transitionary Power|A temporary power enabling the Multisig to operate under the mandate of YIP-41 until the set of decision-making powers covers all needed transactions|


## Future Implementations 

Yearn is continuously paving the way towards an ideal balance of DAO decentralization and productivity. The current phase of efforts impliment changes mostly on the social layer, and in the future we will be moving towards software implementations such as: 

- Multisig consensus mechanisms that allows each yTeam to have execution power 
- Move from proxy voting to on-chain voting
- tokenize decision-making powers as NFTs
- Utilize [Coordinape](https://coordinape.com/) for things like budget allocation and compensation
