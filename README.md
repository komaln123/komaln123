- 👋 Hi, I’m @komaln123
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
komaln123/komaln123 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

    threshold=50 

face_similarity= np.round((100 - (matchPercentage[0] * 100)), 2)


 result = fr.compare_faces(faceOneEcho, faceTwoEcho)[0]
    if result or face_similarity >= threshold:
        print("Face matched.")
        print("face_similarity",face_similarity )
        return {"status": True, "message": "Face match", "data": {"face_similarity": np.round((100 - (matchPercentage[0] * 100)), 2)}}

 else:
        print("Face Unmatched")
        print("face_similarity",face_similarity )
        return {"status": False, "message": "Face unmatch", "data": {"face_similarity": np.round((100 - (matchPercentage[0] * 100)), 2)}}
