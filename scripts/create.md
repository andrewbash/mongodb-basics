# Create

### insertOne()

db.books.insertOne(
{  isbn : "2345678901", title  : "Functional Programming in Scala 9", description : "Functional Programming in Scala is a serious tutorial for programmers looking to learn FP and apply it to the everyday business of coding.", edition : 2016, classifications : ["Technology", "Programming", "Development"], editorial : "Manning Pubns Co.", authors : [ { name : "Paul Chiusano", biography: "Has been writing and shipping functional code in Scala since 2008" }, { name : "Runar Bjarnason", biography: "Is a self-taught programmer with 12 years of industry experience" } ]}
);

### insertMany()

db.books.insertMany([
{  isbn : "1234567890",  title : "Functional Programming in Scala 0", description : "Functional Programming in Scala is a serious tutorial for programmers looking to learn FP and apply it to the everyday business of coding.",  edition : 2014, classifications : ["Technology", "Programming"],  editorial : "Manning Pubns Co.", authors : [ { name : "Paul Chiusano", biography: "Has been writing and shipping functional code in Scala since 2008" }, { name : "Runar Bjarnason", biography: "Is a self-taught programmer with 12 years of industry experience" }] },
{  isbn : "0123456789", title  : "Functional Programming in Scala 1", description : "Functional Programming in Scala is a serious tutorial for programmers looking to learn FP and apply it to the everyday business of coding.", edition : 2012, classifications : ["Technology", "Programming", "Reactive"], editorial : "Manning Pubns Co.", authors : [ { name : "Paul Chiusano", biography: "Has been writing and shipping functional code in Scala since 2008" }, { name : "Runar Bjarnason", biography: "Is a self-taught programmer with 12 years of industry experience" } ]},
{  isbn : "9012345678", title  : "Functional Programming in Scala 2", description : "Functional Programming in Scala is a serious tutorial for programmers looking to learn FP and apply it to the everyday business of coding.", edition : 2016, classifications : ["Technology", "Programming", "Development"], editorial : "Manning Pubns Co.", authors : [ { name : "Paul Chiusano", biography: "Has been writing and shipping functional code in Scala since 2008" }, { name : "Runar Bjarnason", biography: "Is a self-taught programmer with 12 years of industry experience" } ]}
]);
db.books.insertMany([
{  isbn : "8901234567", title  : "Functional Programming in Scala 3", description : "Functional Programming in Scala is a serious tutorial for programmers looking to learn FP and apply it to the everyday business of coding.", edition : 2015, classifications : ["Technology", "Programming", "Reactive"], editorial : "Manning Pubns Co.", authors : [ { name : "Paul Chiusano", biography: "Has been writing and shipping functional code in Scala since 2008" }, { name : "Runar Bjarnason", biography: "Is a self-taught programmer with 12 years of industry experience" } ]},
{  isbn : "7890123456", title  : "Functional Programming in Scala 4", description : "Functional Programming in Scala is a serious tutorial for programmers looking to learn FP and apply it to the everyday business of coding.", edition : 2015, classifications : ["Technology", "Programming", "Frameworks"], editorial : "Manning Pubns Co.", authors : [ { name : "Paul Chiusano", biography: "Has been writing and shipping functional code in Scala since 2008" }, { name : "Runar Bjarnason", biography: "Is a self-taught programmer with 12 years of industry experience" } ]},
{  isbn : "6789012345", title  : "Functional Programming in Scala 5", description : "Functional Programming in Scala is a serious tutorial for programmers looking to learn FP and apply it to the everyday business of coding.", edition : 2005, classifications : ["Technology", "Programming", "Reactive"], editorial : "Manning Pubns Co.", authors : [ { name : "Paul Chiusano", biography: "Has been writing and shipping functional code in Scala since 2008" }, { name : "Runar Bjarnason", biography: "Is a self-taught programmer with 12 years of industry experience" } ]}
]);
db.books.insertMany([
{  isbn : "5678901234", title  : "Functional Programming in Scala 6", description : "Functional Programming in Scala is a serious tutorial for programmers looking to learn FP and apply it to the everyday business of coding.", edition : 1999, classifications : ["Technology", "Programming", "Concurrent"], editorial : "Manning Pubns Co.", authors : [ { name : "Paul Chiusano", biography: "Has been writing and shipping functional code in Scala since 2008" }, { name : "Runar Bjarnason", biography: "Is a self-taught programmer with 12 years of industry experience" } ]},
{  isbn : "4567890123", title  : "Functional Programming in Scala 7", description : "Functional Programming in Scala is a serious tutorial for programmers looking to learn FP and apply it to the everyday business of coding.", edition : 2001, classifications : ["Technology", "Programming", "Reactive"], editorial : "Manning Pubns Co.", authors : [ { name : "Paul Chiusano", biography: "Has been writing and shipping functional code in Scala since 2008" }, { name : "Runar Bjarnason", biography: "Is a self-taught programmer with 12 years of industry experience" } ]},
{  isbn : "3456789012", title  : "Functional Programming in Scala 8", description : "Functional Programming in Scala is a serious tutorial for programmers looking to learn FP and apply it to the everyday business of coding.", edition : 2007, classifications : ["Technology", "Programming", "Reactive"], editorial : "Manning Pubns Co.", authors : [ { name : "Paul Chiusano", biography: "Has been writing and shipping functional code in Scala since 2008" }, { name : "Runar Bjarnason", biography: "Is a self-taught programmer with 12 years of industry experience" } ]}
]);

### mongoimport command

Use *mongoimport* command to import JSON format "documents" to a collection in a database.

mongoimport --db test --collection test --file <your path>/books.json
