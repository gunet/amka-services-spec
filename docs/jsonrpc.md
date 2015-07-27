# AMKA Services JSON-RPC API – Release 1 [DRAFT]

## Warning

This is a work in progress, expect it to change.

## Introduction

JSON-RPC is to JSON, what XML-RPC is to XML,  is way to call remote procedures
over the web. Implementations of JSON-RPC exist in many languages, including
Java, Python, Perl, Ruby, etc.

## Versions Supported

The API supports [JSON-RPC 2.0][jsonrpc]. It is intended to be fully consistent with the [JSON-RPC 2.0 Specification][jsonrpcspec] and [JSON][].

## HTTP details

Using the API is only possible over HTTPS.

All calls are made via the `POST` method.

The base URL for configuring your JSON-RPC client is `https://funhub-devel.gunet.gr/amka-services/`. Requests to this endpoint should have a `Content-Type` header of `application/json-rpc`.

The server will respond with a `HTTP 200` code if the request was succesfull.

If an error occurs, the API returns a response in which the error property contains details about the errors, with the following attributes:

code
    A  number that determines which error occured.
message
    A human-readable error message suitable for display to the user, in English.

## API Methods

TODO

  [jsonrpc]: http://www.wikipedia.org/wiki/JSON-RPC
  [jsonrpcspec]: http://www.jsonrpc.org/specification
  [JSON]: http://www.ietf.org/rfc/rfc4627.txt
