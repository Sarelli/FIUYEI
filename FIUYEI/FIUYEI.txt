#include <iostream>
#include <string>
using namespace std;

string m_characterName; //m_ stands for global variable
string m_choice;


void CheckForError() {

    while (m_choice != "a" && m_choice != "A" && m_choice != "b" && m_choice != "B" && m_choice != "c" && m_choice != "C") 
    {
        cout << "Try again.\n";
        cin >> m_choice;
    }
}

int BadEnding() {
    cout << "You move West. You run for 2 miles and find a green gate.\nThis is it! You can smell your freedom.\nYou go beyond the bars, you're out!\n" <<
        "You don't realise that the cleaning truck is about to suck you into its trash compactor. Few seconds after it hits you.\nGAME OVER\n";
    return 0;
}
    
int main()
{
    cout << "Hello and welcome to 'Fake It Until You Escape It'.\nThis is a questioned based adventure game in which your choices count!\n";
    cout << "But first, choose a name for your character: \n";
    cin >> m_characterName;
    cout << "Perfect, you will be now referred as " << m_characterName << " The Chameleon.\n";

    cout << "...\nIt's night time at London Zoo and everybody is getting ready to leave. EVERYBODY.\n";
    cout << "You are quietly waiting in your tank for your opportunity.\nThe clock strikes 8pm and immeadiately after the fire alarm goes off.\nAll the cages open up and you can finally escape!\n";
    
    cout << "You notice a guard walking towards your tank. How do you proceed:\n"
        << "A. You camouflage with the tree branch in your tank\n"
        << "B. You leap onto the guard sleeve and blend with his shirt\n"
        << "C. You make a break for it\n";
    cin >> m_choice;

    CheckForError();

    if (m_choice == "a" || m_choice == "A") {
        cout << "You decide to stay on your branch but unfortunately the guard locks your door.\nGAME OVER\n";
        return 0;
    }
    else if (m_choice == "b" || m_choice == "B") {
        cout << "The guard doesn't notice you and you make it out of the vivarium.\n";
    }
    else if (m_choice == "c" || m_choice == "C") {
        cout << "You manage to get to the ground but the guard starts chasing you.\nYou decide to:\n"
            << "A. Turn right\n"
            << "B. Turn left\n"
            << "C. Run up the wall\n";
        cin >> m_choice;

        CheckForError();

        if (m_choice == "a" || m_choice == "A") {
            cout << "Your bold decision brings you straight in the snake area.\nYour first encounter is Python Pete.\n";
            cout << "'You think you can e$$cape without my help? You are in$$ane. Jump between my fang$$ and we will make it to the real world'\n";
            cout << "You decide to:\n"
                << "A. Trust him\n"
                << "B. Don't trust him\n"
                << "C. Run away\n";
            cin >> m_choice;

            CheckForError();

            if (m_choice == "a" || m_choice == "A") {
                cout << "You jump in his mouth but as everyone would expect a sneaky snake to act, he closes it and swallows you.\n";
                cout << "You then decide to:\n"
                    << "A. Wait and see what happens\n"
                    << "B. Fight for your life\n";
                cin >> m_choice;

                while (m_choice != "a" && m_choice != "A" && m_choice != "b" && m_choice != "B") {
                    cout << "Try again.\n";
                    cin >> m_choice;
                }

                if (m_choice == "a" || m_choice == "A") {
                    cout << "After few minutes you notice a ray of light. Pete is opening his mouth to let you out.\n'$$ee, I am not that bad after all.'\n";
                }
                else {
                    cout << "You relieve yourself in his stomach to make him feel sick. It works!\n'What the hell  man?! I would have carried you out hone$$tly! $$ort out your$$elf.\n";
                }
            }
            else if (m_choice == "b" || m_choice == "B") {
                cout << "'I don't trust snakes. If you want to join me in escaping I will have to sit on your head.'\nPete understands your point and lets you on his head.\n";
                cout << "You both reach the exit but a python doesn't really get unnoticed. The guard takes him from the tail and pulls him back.\nYou are quick enough to jump off before he catches you too.\n";
            }
            else if (m_choice == "c" || m_choice == "C") {
                cout << "You run back to your corridor but the guard is still there. He throws his net at you and catches you.\nGAME OVER\n";
                return 0;
            }
        }
        else if (m_choice == "b" || m_choice == "B") {
            cout << "You suddenly remembered that your neighbour and best friend John the gecko can see the entrance from his tank, so you run towards him.\n";
            cout << "You arrive at his tank. You decide to:\n"
                << "A. Speak to him\n"
                << "B. Keep running\n";
            cin >> m_choice;

            while (m_choice != "a" && m_choice != "A" && m_choice != "b" && m_choice != "B") {
                cout << "Try again.\n";
                cin >> m_choice;
            }

            if (m_choice == "a" || m_choice == "A") {
                cout << "'Yo man! What are you doing here?'\n'Run away with me! We can escape the zoo tonight and live a great life!'\n'Cheers bro, but I have free food and care in here, ain't going anywhere soz. Good luck tho!'\n";
                cout << "You wonder for a second if you should remain too. But this is a once in a lifetime opportunity.\n";
            }
            cout << "With sadness you say goodbye forever to your friend and move towards the exit\n";
            }
        else if (m_choice == "c" || m_choice == "C") {
            cout << "To blend in you decide to change your skin colour. It's quite dark so you don't know what to choose.\n"
                << "A. White\n"
                << "B. Red\n"
                << "C. Blue\n";
            cin >> m_choice;

            CheckForError();

            if (m_choice == "a" || m_choice == "A") {
                cout << "The guard points his torch to the wall, but can't see you on it. You got the correct colour!\nYou walk along the wall until you find the exit door.\n";
            }
            else {
                cout << "The guard points his torch to the white wall and can easily spot you.\nGAME OVER\n";
                return 0;
            }
            
        }

    }

    cout << "It's quite chilly outside, so you decide to move towards the Savannah zone.\nYou don't know exactly where it is, so you decide to:\n"
        << "A. Turn left\n"
        << "B. Turn right\n"
        << "C. Look at the visitors map in front of you\n";
    cin >> m_choice;

    CheckForError();

    if (m_choice == "a" || m_choice == "A") {
		cout << "You move West. You run for 2 miles and find a green gate.\nThis is it! You can smell your freedom.\nYou go beyond the bars, you're out!\n" <<
			"You don't realise that the cleaning truck is about to suck you into its trash compactor. Few seconds after it hits you.\nGAME OVER\n";
    }
    else if (m_choice == "b" || m_choice == "B") {
        cout << "The zoo is shaped like a circle, therefore you should be able to reach your frind Tina sooner or later.\n";
        cout << "You arrive at the tigers cage.\n" << "'Tina' you shout.\nA majestic fluffy creature jumps at you.\n"
            << "A. You mimetise yourself to escape the predator\n"
            << "B. You run\n"
            << "C. Tina?\n";
        cin >> m_choice;

        CheckForError();

        if (m_choice == "a" || m_choice == "A") {
            cout << "Not seeing anyone, the fearless animal goes back to its corner.\nKeeping your cover, you make your move to the zoo gate.\n";
            BadEnding();
        }
        else if (m_choice == "b" || m_choice == "B") {
            BadEnding();
        }
        else if (m_choice == "c" || m_choice == "C") {
            cout << "It's Tina The Tiger.\nYou and her jump the wall and make it to the real world. No one can stop you guys now.\nYOU WIN\n";
        }
    }
    else if (m_choice == "c" || m_choice == "C") {
        cout << "The map is lit up with some neon lights that make you very visible to the guard passing by.\nGAME OVER\n";
        return 0;
    }

    return 0;
}

