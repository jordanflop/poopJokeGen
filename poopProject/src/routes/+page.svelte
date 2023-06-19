<script>

let joke = "press the above button";

let buttonText = "press me, just do it"

const jokes = ["Why couldn't the poop cross the road? Because it got stuck in a crack!", "What goes click-click-click-splat? A dangerous poop!", "Why did the poop emoji feel embarrassed? Because it had a crappy job!", "What do you call it when a poop tries to be funny? A wisecrapp!", "Why did the poop go to the movies? It wanted to see The Dark Knight Squats!", "How do you know if a poop is feeling down? It looks a little browned off!", "What did one poop say to the other poop in the toilet bowl? You look flushed!", "What do you call a poop that's trying to be healthy? A green movement!"];

function newJoke() {
    let random = Math.floor(Math.random() * jokes.length);
    joke = jokes[random];
    console.log(joke);
    if (buttonText == "press me, just do it") {
        buttonText = "press me again, I dare you";
    }
}


</script>


<main>

<p id="title">💩 Joke generator</p>


<button on:click={newJoke}>{buttonText}</button>
<p id="joke">{joke}</p>


</main>

<style>

#title {
    background: linear-gradient(to right, #544a7d, #ffd452);
    width: 25%;
    font-size: 300%;
    border-radius: 15px;
    position: absolute;
    left: 37.5%;
    font-weight: 700;
    text-align: center;
    transition: background 3s;
}

#title:hover {
    background: linear-gradient(to right, #f4791f, #659999); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

}

button {

    background: linear-gradient(to right, #2ebf91, #8360c3); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

    position: absolute;
    top: 25%;
    width: 10%;
    font-size: 100%;
    border-radius: 15px;
    position: absolute;
    left: 45%;
    font-weight: 700;
    text-align: center;
    height: 5%;
}

button:hover {
    left: 43.75%;
    width: 12.5%;

}

#joke {
    position: absolute;
    top: 40%;
    width: 100%;
    left: 0%;
    font-size: 250%;
    font-weight: 1000;
    color: chocolate;
    text-align: center;
}


</style>