# Copyright 2016 Pants project contributors (see CONTRIBUTORS.md).
# Licensed under the Apache License, Version 2.0 (see LICENSE).

files(
  name = 'junit_xml',
  sources = rglobs('junit_xml/*.xml'),
)

python_tests(
  sources = ['test_junit_html_report.py'],
  dependencies = [
    ':junit_xml',
    'src/python/pants/backend/jvm/tasks/reports',
    'src/python/pants/util:contextutil',
    'src/python/pants/util:strutil',
    'tests/python/pants_test:test_infra',
  ],
  tags = {'partially_type_checked'},
)
