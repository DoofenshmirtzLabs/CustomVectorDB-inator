# CustomVectorDB
Project Description:

This project implements a lightweight vector database system for storing user data in files. It leverages sentence embeddings to represent user data from documents like PDFs, Word files, and presentations. Here's a breakdown of the functionalities:

User Data Storage:
fetch_user_dict retrieves a user's data dictionary from a JSON file.
save_user_dict saves a user's data dictionary to a JSON file.
Embedding Management:
post_embeddings stores page embeddings for a specific book (file) in the user's data.
retrieve_topk searches for the most similar documents (books) based on a query embedding.
Content Processing:
get_embeddings generates sentence embeddings from textual content.
read_content extracts text content from different file formats and generates embeddings for each page.
Key Points:

This system doesn't use a traditional database but leverages files for user data storage.
Vector embeddings provide a compact and efficient way to represent document content.
The system facilitates similarity search based on user data embeddings.
Note: This is a file-based system, not a full-fledged vector database solution.
key Function Names:

fetch_user_dict(user_id)
save_user_dict(user_id, data)
post_embeddings(user_id, book_id, embeddings, page_no)
retrieve_topk(query_embeddings, user_dict, top_k)
get_embeddings(text)
read_content(file_path, file_name, UserID)

