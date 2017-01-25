FROM microsoft/dotnet:1.1-sdk-msbuild

# Create directory for the app source code
RUN mkdir -p /usr/src/core
WORKDIR /usr/src/core

# Copy the source and restore dependencies
COPY . /usr/src/core
RUN dotnet restore

# Expose the port and start the app
EXPOSE 5000
CMD [ "dotnet", "run" ]