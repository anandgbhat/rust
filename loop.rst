#![allow(dead_code)]

fn try_while()
{
	let mut x = 1;

	while x <= 5 {
		println!("x = {} ", x);
		x = x+1;
	}
}


fn try_loop() {
	let mut x = 100;
	loop {
		x = x/5;
		if x == 0 {
			break;
		} else {
			println!("x = {}", x);
		}
	}
}
		

fn main() 
{
	try_while();
	println!("#######################");
	try_loop();
}
