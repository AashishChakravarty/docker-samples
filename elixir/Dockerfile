# Start with an official Elixir runtime as a parent image
FROM elixir:1.12.1

# Set the working directory for the Docker container
WORKDIR /app

# Copy the mix.exs and mix.lock files to the container
COPY mix.exs mix.lock ./

# Install the dependencies
RUN mix local.hex --force && \
    mix local.rebar --force && \
    mix deps.get

# Copy the rest of the application files to the container
COPY . .

# Compile the Elixir application
RUN mix compile

# Expose the port that the Phoenix application will run on
EXPOSE 4000

# Run the Phoenix application with mix
CMD ["mix", "phx.server"]