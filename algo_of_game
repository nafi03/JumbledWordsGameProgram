import random

def choose():
    #List of the words that are used.Can be changed according to you. 
    words=["umbrella","america","programming","debugging","festival","holidays","randomly","permutation","combination","outstanding","wonders","chocolate","cricket","football","volleyball","smartphone","smartwatch","facebook","instagram"]
    chosen=random.choice(words)
    return chosen
    
def jumbled(words):
    jumbled="".join(random.sample(words, len(words)))
    return jumbled
    
def play_game():
    
    turn=0
    score1=0
    score2=0
    p1=input("Player 1, Please enter your name:",)
    p2=input("Player 2, Please enter your name:",)
  
    while(1):
        word=choose()
        W=jumbled(word)
        print("\n",W,"\n")
        
        if(turn%2==0):
            print(p1,"'s turn.")
            p1ans=input("Guess the word I am thinking...",)
        
            if(p1ans==word):
                score1=score1+1
                print("Correct! Your score is:",score1)
            else:
                print("Unfortunately that was Incorrect.The word I thought was:",word,"\n Your score remains:",score1)
            
        else:
            print(p2,"'s turn.")
            p2ans=input("Guess thee word I am thinking....",)
            if(p2ans==word):
                score2=score2+1
                print("Correct! Your score is:",score2)
            else:
                print("Unfortunately that was Incorrect.The word I thought was:",word,"\n Your score remains:",score2)
            c=input("If you want to continue press 1 for yes 0 for no.",)
            if (c=="0"):
                print("Thank you for playing with us.",p1,"and",p2,"Your scores are:",score1,",",score2,"respectively.")
                break
        turn=turn+1
        
play_game()
