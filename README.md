# two-of-a-kind
This project was to demonstrate our skills in how to use onEvent functions and how they can be used to make a choose your own adventure game application. I took inspiraition from games I would play as a child and thought I would recreate it for an assignment.

playSound("sound://category_loops/vibrant_game_musical_harping_movement_loop_1.mp3", false);
onEvent("startButton", "click", function( ) {
  setScreen("screen1");
  onEvent("button1", "click", function( ) {
    setScreen("screen2");
    onEvent("button4", "click", function( ) {
      setScreen("screen4");
      //remember to make new screen for this option (this is the hangup button)
      onEvent("button8", "click", function( ) {
        setScreen("screen2");
      });
      onEvent("button9", "click", function( ) {
        setScreen("homeScreen");
      });
    });
    onEvent("button5", "click", function( ) {
      setScreen("screen5");
      onEvent("button10", "click", function( ) {
        setScreen("homeScreen");
      });
      onEvent("button11", "click", function( ) {
        setScreen("screen6");
        onEvent("button12", "click", function( ) {
          setScreen("screen7");
          onEvent("button14", "click", function( ) {
            setScreen("screen8");
            onEvent("button16", "click", function( ) {
              setScreen("screen9");
              onEvent("button17", "click", function( ) {
                setScreen("screen10");
                onEvent("button18", "click", function( ) {
                  setScreen("screen11");
                  onEvent("button20", "click", function( ) {
                    setScreen("screen12");
                    onEvent("button21", "click", function( ) {
                      setScreen("homeScreen");
                    });
                  });
                });
                onEvent("button19", "click", function( ) {
                  setScreen("screen13");
                  //make new screen for "button19"
                  onEvent("button22", "click", function( ) {
                    setScreen("screen10");
                  });
                  onEvent("button23", "click", function( ) {
                    setScreen("homeScreen");
                  });
                });
              });
            });
          });
        });
        onEvent("button13", "click", function( ) {
          setScreen("homeScreen");
        });
      });
    });
  });
  onEvent("button2", "click", function( ) {
    setScreen("screen3");
    onEvent("button6", "click", function( ) {
      setScreen("screen1");
      onEvent("button7", "click", function( ) {
        setScreen("homeScreen");
      });
    });
  });
});
