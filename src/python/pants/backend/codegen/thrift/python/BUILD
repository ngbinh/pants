# Copyright 2016 Pants project contributors (see CONTRIBUTORS.md).
# Licensed under the Apache License, Version 2.0 (see LICENSE).

python_library(
  dependencies = [
    # Note that this is part of a gnarly dependency chain:
    #  backend/python:thrift_builder ->
    #  backend/codegen/thrift/python ->
    #  backend/python/targets:python
    # This isn't circular, but it's still bad that it crosses between backends and back again.
    # TODO: Clean this up. thrift_builder should almost certainly be in the codegen backend.
    'src/python/pants/backend/python/targets:python',
  ],
)
