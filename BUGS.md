# pythonProjectPetFriends test 24.7.2
БАГИ!

Список тестов, которые должны проваливаться (получать статус "FAILED"), но проходят (получают статус "PASSED"):
- test_add_new_pet_with_photo_and_empty_data(name='', animal_type='', age='', pet_photo='images/Dogsad.jpg')
- test_add_new_pet_without_photo_and_with_empty_data(name='', animal_type='', age='')
- test_add_new_pet_with_incorrect_age(name='Thomas', animal_type='Hide cat', age='-2', pet_photo='images/trueTom.jpg')
- test_update_not_own_pet_info(name='Viktriks', animal_type='Shlepa', age='4')

Список тестов, которые должны получать статус-код "500", а получают - "200":
- test_set_photo_not_own_pet(pet_photo='images/deer.jpg')
