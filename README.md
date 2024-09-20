# rustactixsqlxsimplecrud

is a code for learning rust purpose based this url https://codevoweb.com/rust-build-a-crud-api-with-sqlx-and-postgresql/

first add crates dependency

cargo add actix-web
cargo add actix-cors
cargo add serde_json
cargo add serde --features derive
cargo add chrono --features serde
cargo add env_logger
cargo add dotenv
cargo add uuid --features "serde v4"
cargo add sqlx --features "runtime-async-std-native-tls postgres chrono uuid"

running docker compose

docker-compose up -d

then install sqlx-cli

cargo install sqlx-cli

once instalation done running this script

sqlx migrate add -r init

write table create sql in init_up.sql then

sqlx migrate run
