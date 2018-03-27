# frozen_string_literal: true

# Copyright (C) 2018 Sandro Jäckel.  All rights reserved.
#
# This file is part of Canuby.
#
# Canuby is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
#
# Canuby is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with Canuby.  If not, see <http://www.gnu.org/licenses/>.
require 'rdoc/task'
require 'rake/testtask'

TESTOPTS = '--profile'

Rake::TestTask.new do |t|
  t.libs << 'test'
end

RDoc::Task.new do |rdoc|
  rdoc.title = 'Canuby'
  rdoc.main = 'README.md'
  rdoc.rdoc_files = FileList.new %w[lib LICENSE README.md]
  rdoc.rdoc_dir = 'docs'
  rdoc.markup = 'markdown'
  rdoc.options << '--exclude=3rdparty'
end

task default: :test
