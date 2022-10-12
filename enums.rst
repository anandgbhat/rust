#![allow(dead_code)]
#![allow(unused_variables)]

enum PlayingStyle {
	Batsman,
	Bowler,
	Allrounder
}

struct Player {
	name: String,
	style: PlayingStyle
}

fn style_str(p : PlayingStyle) -> String {
	match p {
		PlayingStyle::Batsman => return "Batsman".to_string(),
		PlayingStyle::Bowler => return "Bowler".to_string(),
		PlayingStyle::Allrounder =>  return "Allrounder".to_string(),
	}
}

fn main() {
	let player1 = Player{ name: "Sachin Tendulkar".to_string(),  style: PlayingStyle::Allrounder};
	let player2 = Player{ name: "Ricky Ponting".to_string(), style: PlayingStyle::Batsman};

	println!("Player {} is {} ", player1.name, style_str(player1.style));
	println!("Player {} is {} ", player2.name, style_str(player2.style));
}
	
