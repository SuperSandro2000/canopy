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
require 'rake/testtask'
require 'rdoc/task'

require_relative 'lib/canuby'

Rake::TestTask.new do |t|
  t.libs << 'test'
end

RDoc::Task.new do |doc|
  doc.title  = 'Canuby'
  #doc.rdoc_files = FileList.new %w[lib LICENSE README]
  rdoc.markup = 'markdown'
  doc.rdoc_dir = 'doc'
end

task default: :test
