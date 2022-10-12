#![allow(dead_code)]
#![allow(unused_variables)]

fn check_match() {
	let country_code = 1;

	let country = match country_code {
		1 => "USA",
		44 => "UK",
		46 => "Sweden",
		91 => "India",
		_ => "invalid"
	};

	println!("the country with code {} is {} ",
		country_code, country);
}

fn main() {
	check_match()
}
