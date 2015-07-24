# README

## Installing

After checking out the repository, run:

```
docker-compose build
docker-compose run web bin/rake db:create db:migrate
```

## Testing

Initialize the DB by running:

```
docker-compose run web bin/rake db:create db:migrate RAILS_ENV=test
```


## Usage

With Docker Compose you can run a container with an attached TTY, which allows
to use tools like `pry` for debugging:

```
docker-compose run --service-ports web
```

