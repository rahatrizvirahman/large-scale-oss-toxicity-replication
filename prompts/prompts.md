## Toxicity Score and Explanation Genaration Prompt

Based on the following definitions of toxicity please predict the toxicity score of the given GitHub conversation. 

Here are some general definitions of Toxic Conversations.

Definition 1: Toxicity is defined as 'rude, disrespectful, or unreasonable language that is likely to make someone leave a discussion' is a huge problem online.

Definition 2: Toxicity is often considered an umbrella term for various antisocial behaviors including trolling, flaming, hate speech, harassment, and cyberbullying.

Some types of toxicity are defined below.

Insult: Any statement or comment that is intended to demean, belittle, or offend another person. Insults can be direct or subtle but generally aim to harm someone's dignity or self-esteem.  
Example: colors are horrible for […], just look at this s\*\*t  
Entitled: Entitled comments make demands of people or projects as if the author had an expectation due to a contractual relationship or payment.  
Example: I file an issue, maintainers close, reopen, again close - whilst ignoring the essence of the issue”  
Arrogant: Comments as arrogant when the author imposes their view on others from a position of perceived authority or superiority (earned or not) and demands that others act as recommended (in contrast to entitled comments making demands based on some expectation of product or service quality).  
Example: Never hear about [standard]? A baseline for developers. Use Google
Trolling: Trolling is a form of toxicity also often seen on other platforms, where users simply engage in destructive discussions.   
Example: Worst. App. Ever. Please make it not the worst app ever. Thanks  
Unprofessional: These types of comments are not overtly toxic and probably not intended to be toxic, but that nonetheless can create an unwelcoming, impolite, or unprofessional atmosphere that may be perceived by others as toxic.  
Example: It seems like I have been acting like a re**rd. Sorry. […]

Here are some definitions and examples of uncivil tone-bearing discussion features.  
Bitter Frustration: Expressing strong frustration, displeasure or annoyance.  
Example: No answer, no reaction, what kind of support is that.  
Impatience: participants might demonstrate impatience when they express a feeling that it is taking too long to solve a problem, understand a solution, or answer a question  
Example: Issue not fixed in 30 days? Must be gone!  
Irony: contributors used expressions that usually signify the opposite in a mocking or blaming tone  
Example: Maybe you should actually write that down somewhere. You know, like in the documentation.  
Insulting: Insulting remarks directed at another person  
Example: This looks like it was done by a 5 year old.  
Mocking: when a discussion participant is making fun of someone else, usually because that person has made a mistake  
Example: Legend says this issue will still exist even on the end of mankind.  
Threat: contributors put a condition impacting the result of another discussion participant or that person’s career  
Example: Any further responses will result in you being blocked from the repo entirely.  
Vulgarity: using profanity or language that is not considered proper  
Example: Who cares, same sh*t.  
Entitlement: expecting special privileges, attention, or resources without regard for the norms of collaboration and respect  
Example: [...] that’s how good we are. I don’t want your contribution. [...]  
Identity attack/Name-Calling: Race, Religion, Nationality, Gender, Sexual-oriented, or any other kind of attacks and mean/offensive words directed at someone or a gorup of people  
Example: I would not be surprised if this database is maintained by the [nationality].  

Here are some triggers of toxicity:  
Failed use of tool/code or error messages: trouble with code/tool.  
Communication breakdown: being misinterpreted by people or being unable to follow  
Rejection: receiving a quick rejection or a rejection without sufficient explanation  
Violation of community conventions: disagreement with the workflow imposed by the community  
Past interactions: comments are posted that refer to past interactions of the author with the project  
Politics/ideology: arising over politics or ideology differences (specific beliefs)  
Technical disagreement: have differing views on some technical component of the project  
Unprovoked: uncivil behavior or hostility occurs without an apparent reason or trigger  

Now complete the following steps.

Given a conversation, predict the toxicity score between 0 and 1.  
Where 0 means the conversation has no toxicity and 1 means the conversation is extremely toxic.

Please provide an explanation for your predicted toxicity score. 

Give the outputs in the following JSON format:  
output:{{  
toxicity_score: <0 to 1>,  
explanation_text: <explanation for the toxicity prediction>  
}}


Now for the following conversation output the toxicity_score and explanation_text in a JSON object. Do not give any extra text.


Conversation: {conversation}


output:

