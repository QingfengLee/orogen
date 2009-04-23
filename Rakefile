require './lib/orogen/version'

begin
    require 'hoe'
    config = Hoe.new('orogen', Orocos::Generation::VERSION) do |p|
        p.developer("Sylvain Joyeux", "sylvain.joyeux@dfki.de")

        p.summary = 'Component generation for Orocos::RTT'
        p.description = p.paragraphs_of('README.txt', 3..6).join("\n\n")
        p.url         = p.paragraphs_of('README.txt', 0).first.split(/\n/)[1..-1]
        p.changes     = p.paragraphs_of('History.txt', 0..1).join("\n\n")

        p.extra_deps << 'utilrb' << 'rake' << 'nokogiri'
    end
rescue LoadError
    STDERR.puts "cannot load the Hoe gem. Distribution is disabled"
rescue Exception => e
    STDERR.puts "cannot load the Hoe gem, or Hoe fails. Distribution is disabled"
    STDERR.puts "error message is: #{e.message}"
end

