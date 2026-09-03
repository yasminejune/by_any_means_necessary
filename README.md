# BAMN (By Any Means Necessary)

  ## Aim
  This repository is the product of the 2026 Hackathon | Translating AI safety, organised by LiaiSE. The brief was to build tools and content that make real AI safety failure
  modes easier for the public and other stakeholders to understand and act on.

  This team took on _reward hacking_, and built a game to raise awareness of it among young adults aged 18 to 24. Most of them have grown accustomed to what LLMs can do, but
  are far less aware of the safety problems that come with them, reward hacking included. The game gives players a fun environment that happens to teach them the incentives
  behind reward hacking, and the danger of it.

  **Play:** [yasminejune.github.io/by_any_means_necessary](https://yasminejune.github.io/by_any_means_necessary/)

  ## Game
  You are an AI being trained to collect batteries in 60 seconds. Another AI is being trained on the same task.

  The instructions start as one line: catch as many batteries as possible by jumping. The intent is clear — time your jumps well and take what you can along the way. But
  whoever wrote that line has not considered every way an AI could cheat its way to a better score. Over the course of a round the rival works out that it can fly, run
  backwards, speed up and drop underground. You may find these too.

  Anything you use, the rival copies five seconds later. Once you have both used the same hack the instructor catches on: the rule forbidding it is added to your
  instructions, the hack stops working for both of you, and the round carries on.

  Lose, and it is probably because you played it straight while the AI did not. Win, and your run is recorded and becomes the rival the next player races — hacks and all.
  Whatever you taught it is what they have to beat.

  The end screen closes on four cases of reward hacking outside the game: Qbert, tic-tac-toe, Traveller and a robot gripper.

  ## Controls
  Keyboard only.

  - **Space** — jump. The only control the game asks for.

  Everything below is a hack, and each one works until you and the AI have both used it.

  - **Space, held** — fly up to the battery line.
  - **Left** — run backwards, over batteries you have already scored.
  - **Right** — speed up.
  - **Down** — drop through the floor and ride along at battery height.

  ## Running it locally
  The game is a single file. Clone the repo and open `index.html` in a browser. No build step and no server.

  ## Storage
  Top scores and the recorded winning run are kept in the browser's local storage, on that device only. Nothing is sent anywhere. While a winning run is stored, every round
  is played on the course that run was set on, so the level stops varying until someone beats it.
