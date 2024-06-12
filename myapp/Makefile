verify:
	# shows compute cap (recommended >8)
	nvidia-smi --query-gpu=compute_cap --format=csv
	# shows cuda version (recommended 11.0)
	nvcc --version

build:
	cargo build

rust-version:
	@echo "Rust command-line utility versions:"
	rustc --version 			#rust compiler
	cargo --version 			#rust package manager
	rustfmt --version			#rust code formatter
	rustup --version			#rust toolchain manager
	clippy-driver --version		#rust linter

format:
	cargo fmt --quiet

lint:
	cargo clippy --quiet

test:
	cargo test --quiet

run:
	cargo run

release:
	cargo build --release

all: format lint test run