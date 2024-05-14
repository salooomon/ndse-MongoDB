запрос(ы) для вставки данных минимум о двух книгах в коллекцию books
db.collection.insertMany([book_1, book_2, ...])

запрос для поиска полей документов коллекции books по полю title,
db.collection('library').find({ title: "название" });

запрос для редактирования полей: description и authors коллекции books по _id записи.
db.collection('library').updateOne(
  { id: '1' },
  {
    $set: {description: "string", authors: "string"}
  }
);