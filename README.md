# i.do - The code-based todo-list
"**i.do**" is a code-based todo-list that focuses on habit building and procedures.

Because sometimes you need an algorithm that works for you, not just a bullet list.

**The plan is: **

- get the app working to automate the task tracking

- get a community to form around this format

- share wisdom and useful algorithms

- create a steady database for all to use

## Example of format

For instance, the below pseudo-code is readable, and anyone can perform it for keeping track of tasks, in a deeper way than simply todo-lists.

The goal is to make an app that automates this process and keeps you on track of your goals.

*"The problem today is not the lack of information, it's the lack of wisdom."*

```
//Learning hyper-parameters, 
// choose your own, 
// know yourself
//
MAX_Tries = 5;                           //Know when to give up in your approach
MAX_lateral_thinking = 10;                                // How many concurrent subjects can be tackled at once during learning
MAX_thinking_depth = 3;                  //How many related subjects should be pursued during learning
world = Universe.getReality()            //This is the world we live and learn in
[me, my, I, I_am] = Universe.myself;     //These refer to you

I.learn ( subject )
{
    //Don't multitask
    if( I_am.currently_learning_count() > MAX_lateral_thinking )
    {
        importance = I.estimate_importance( subject );
        return my.backlog.add_for_later( subject, importance );
    }


    //Start fresh
    new blank_note;
    blank_note.write( world.find_new_research_points( subject ) );


        //Attempt to understand
        tries = 0;
        while ( understand( blank_note )  != true )
        {
            rewrite_in_simple_terms ( blank_note );

            tries++;
            if( tries > maxTries )
            {
                //Research leads nowhere
                return learn( subject );
            }
        }        
         

        //Look to understand related subjects
        if ( related_subjects = world.find_related_subjects(subject) )
    {
        depth = subject.currentDepth();
        if( depth <= MAX_thinking_depth )
        {
            learn( related_subjects )
        }
    }


        //Test to see that you refined the concept
        while ( find_child_and_teach ( blank_note ) != success )
        {
            //Start again
            return learn ( subject );
        }


        //Index the new information
    me.knowledge_base.organize_and_index ( blank_sheet_of_paper );


        //Consolidate already present information
    if ( related_known_subjects = knowledge_base.find_related_subjects( subject ) )
    {
        learn( related_known_subjects );
    }


        //Mark subject as learned
    return me.mark( subject, "learned" )

    //If your current knowledge can be applied 
    if ( my.knowledge
}
```


# Roadmap

## Stage1 - Prototype
### 1. Create the python framework
### 2. Create jupyter notebook prototype that follows simple flow
### 3. Make web interface that accepts i.do lists  
### 4. Make rudimentary control flows
### 5. Decide on a system that knows which "actions" and "tokens" are defined and which are not (and require human input)
### 6. Create action feedback and response, that gets saved for each user.
### 7. Make the flow seamless and easy to use
### 8. Make a MVP, and launch tests.

## Stage2 - Attract the community
### 1. Create social media involvement
### 2. Standardise the format of i.do
### 3. Gather a collection of i.do notes
### 4. Decide on branding and name
### 5. Create & Test & Refine

## Stage3 - Scale the feedback
### 1. Add voting system
### 2. Add local database to store the notes
### 3. Base it all on git
### 4. Create nodes, that people can gather and vote on
