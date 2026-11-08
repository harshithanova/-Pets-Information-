
import 'package:flutter/material.dart';

void main() {
  runApp(const PetWorldApp());
}

class PetWorldApp extends StatelessWidget {
  const PetWorldApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      title: 'Pet World',
      theme: ThemeData(
        colorSchemeSeed: Colors.teal,
        useMaterial3: true,
      ),
      home: const LoginPage(),
    );
  }
}

// ANIMAL DATA
class Animal {
  final String name;
  final String image;
  final String food;
  final String habitat;
  final String lifespan;
  final String description;
  final String fact;

  const Animal({
    required this.name,
    required this.image,
    required this.food,
    required this.habitat,
    required this.lifespan,
    required this.description,
    required this.fact,
  });
}

final List<Animal> animals = [
  Animal(
    name: 'Dog',
    image: 'https://loremflickr.com/500/400/dog',
    food: 'Meat, dog food and vegetables',
    habitat: 'Homes and shelters',
    lifespan: '10-13 years',
    description: 'Dogs are friendly and loyal domestic animals. '
        'They are known as human best friends.',
    fact: 'Dogs have an excellent sense of smell.',
  ),
  Animal(
    name: 'Cat',
    image: 'https://loremflickr.com/500/400/cat',
    food: 'Fish, meat and cat food',
    habitat: 'Homes and natural environments',
    lifespan: '12-18 years',
    description: 'Cats are small, playful and independent pets. '
        'They enjoy sleeping and exploring.',
    fact: 'Cats can rotate their ears to hear sounds.',
  ),
  Animal(
    name: 'Hamster',
    image: 'https://loremflickr.com/500/400/hamster',
    food: 'Seeds, grains and vegetables',
    habitat: 'Burrows and pet cages',
    lifespan: '2-3 years',
    description: 'Hamsters are small furry rodents. '
        'They are popular as household pets.',
    fact: 'Hamsters store food in their cheek pouches.',
  ),
  Animal(
    name: 'Panda',
    image: 'https://loremflickr.com/500/400/panda',
    food: 'Mostly bamboo',
    habitat: 'Mountain forests in China',
    lifespan: '15-20 years in the wild',
    description: 'Giant pandas are famous for their black '
        'and white fur.',
    fact: 'Pandas spend many hours eating bamboo.',
  ),
  Animal(
    name: 'Penguin',
    image: 'https://loremflickr.com/500/400/penguin',
    food: 'Fish, krill and squid',
    habitat: 'Southern Hemisphere',
    lifespan: '15-20 years',
    description: 'Penguins are flightless birds that are '
        'excellent swimmers.',
    fact: 'Penguins use their wings like flippers.',
  ),
  Animal(
    name: 'Hen',
    image: 'https://loremflickr.com/500/400/hen',
    food: 'Grains, seeds and insects',
    habitat: 'Farms and poultry houses',
    lifespan: '5-10 years',
    description: 'Hens are female domestic chickens '
        'that lay eggs.',
    fact: 'A healthy hen can lay many eggs in a year.',
  ),
  Animal(
    name: 'Fish',
    image: 'https://loremflickr.com/500/400/goldfish',
    food: 'Algae, plants and fish food',
    habitat: 'Freshwater and oceans',
    lifespan: 'Varies by species',
    description: 'Fish are aquatic animals that breathe '
        'through gills.',
    fact: 'Fish use their gills to take oxygen from water.',
  ),
  Animal(
    name: 'Parrot',
    image: 'https://loremflickr.com/500/400/parrot',
    food: 'Fruits, seeds and nuts',
    habitat: 'Tropical forests',
    lifespan: '15-80 years, depending on species',
    description: 'Parrots are colorful birds known for '
        'their intelligence.',
    fact: 'Some parrots can imitate human speech.',
  ),
  Animal(
    name: 'Rabbit',
    image: 'https://loremflickr.com/500/400/rabbit',
    food: 'Hay, grass and leafy vegetables',
    habitat: 'Grasslands and homes',
    lifespan: '8-12 years',
    description: 'Rabbits are gentle animals with long '
        'ears and strong back legs.',
    fact: 'Rabbits have continuously growing teeth.',
  ),
  Animal(
    name: 'Turtle',
    image: 'https://loremflickr.com/500/400/turtle',
    food: 'Plants, insects and small animals',
    habitat: 'Land, rivers and oceans',
    lifespan: '50-100+ years for some species',
    description: 'Turtles are reptiles protected by '
        'a hard shell.',
    fact: 'Some turtles can live for more than 100 years.',
  ),
  Animal(
    name: 'Lion',
    image: 'https://loremflickr.com/500/400/lion',
    food: 'Meat',
    habitat: 'Grasslands and savannas',
    lifespan: '10-15 years in the wild',
    description: 'Lions are large wild cats known '
        'for their strength.',
    fact: 'A group of lions is called a pride.',
  ),
  Animal(
    name: 'Elephant',
    image: 'https://loremflickr.com/500/400/elephant',
    food: 'Grass, leaves and fruits',
    habitat: 'Forests and grasslands',
    lifespan: '60-70 years',
    description: 'Elephants are the largest living '
        'land animals.',
    fact: 'Elephants use their trunks to smell, drink '
        'and pick up objects.',
  ),
  Animal(
    name: 'Giraffe',
    image: 'https://loremflickr.com/500/400/giraffe',
    food: 'Leaves and shoots',
    habitat: 'African savannas',
    lifespan: '20-25 years',
    description: 'Giraffes are tall animals with '
        'very long necks.',
    fact: 'Giraffes are the tallest living land animals.',
  ),
  Animal(
    name: 'Monkey',
    image: 'https://loremflickr.com/500/400/monkey',
    food: 'Fruits, seeds and insects',
    habitat: 'Forests and grasslands',
    lifespan: 'Varies by species',
    description: 'Monkeys are intelligent and active '
        'social animals.',
    fact: 'Many monkeys use their tails for balance.',
  ),
  Animal(
    name: 'Butterfly',
    image: 'https://loremflickr.com/500/400/butterfly',
    food: 'Flower nectar',
    habitat: 'Gardens, forests and meadows',
    lifespan: 'Usually 2-4 weeks as an adult',
    description: 'Butterflies are beautiful insects '
        'with colorful wings.',
    fact: 'Butterflies taste using their feet.',
  ),
];

// LOGIN PAGE
class LoginPage extends StatefulWidget {
  const LoginPage({super.key});

  @override
  State<LoginPage> createState() => _LoginPageState();
}

class _LoginPageState extends State<LoginPage> {
  final username = TextEditingController();
  final password = TextEditingController();

  void login() {
    if (username.text.trim().isNotEmpty &&
        password.text.trim().isNotEmpty) {
      Navigator.pushReplacement(
        context,
        MaterialPageRoute(
          builder: (context) => const HomePage(),
        ),
      );
    } else {
      ScaffoldMessenger.of(context).showSnackBar(
        const SnackBar(
          content: Text('Please enter username and password'),
        ),
      );
    }
  }

  @override
  void dispose() {
    username.dispose();
    password.dispose();
    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.teal.shade50,
      body: Center(
        child: SingleChildScrollView(
          padding: const EdgeInsets.all(25),
          child: Column(
            children: [
              const Icon(
                Icons.pets,
                size: 90,
                color: Colors.teal,
              ),
              const SizedBox(height: 15),
              const Text(
                'PET WORLD',
                style: TextStyle(
                  fontSize: 32,
                  fontWeight: FontWeight.bold,
                  color: Colors.teal,
                ),
              ),
              const Text('Discover the world of animals!'),
              const SizedBox(height: 35),
              TextField(
                controller: username,
                decoration: const InputDecoration(
                  labelText: 'Username',
                  prefixIcon: Icon(Icons.person),
                  border: OutlineInputBorder(),
                  filled: true,
                  fillColor: Colors.white,
                ),
              ),
              const SizedBox(height: 20),
              TextField(
                controller: password,
                obscureText: true,
                decoration: const InputDecoration(
                  labelText: 'Password',
                  prefixIcon: Icon(Icons.lock),
                  border: OutlineInputBorder(),
                  filled: true,
                  fillColor: Colors.white,
                ),
              ),
              const SizedBox(height: 25),
              SizedBox(
                width: double.infinity,
                height: 50,
                child: ElevatedButton(
                  onPressed: login,
                  style: ElevatedButton.styleFrom(
                    backgroundColor: Colors.teal,
                    foregroundColor: Colors.white,
                  ),
                  child: const Text(
                    'LOGIN',
                    style: TextStyle(fontSize: 18),
                  ),
                ),
              ),
              const SizedBox(height: 15),
              const Text('Welcome to Pet World 🐾'),
            ],
          ),
        ),
      ),
    );
  }
}

// HOME PAGE
class HomePage extends StatelessWidget {
  const HomePage({super.key});

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: const Text(
          'Pet World 🐾',
          style: TextStyle(fontWeight: FontWeight.bold),
        ),
        backgroundColor: Colors.teal,
        foregroundColor: Colors.white,
      ),
      body: Column(
        crossAxisAlignment: CrossAxisAlignment.start,
        children: [
          const Padding(
            padding: EdgeInsets.all(16),
            child: Text(
              'Explore Animals',
              style: TextStyle(
                fontSize: 24,
                fontWeight: FontWeight.bold,
              ),
            ),
          ),
          const Padding(
            padding: EdgeInsets.symmetric(horizontal: 16),
            child: Text('Tap on an animal to know more about it!'),
          ),
          const SizedBox(height: 12),
          Expanded(
            child: GridView.builder(
              padding: const EdgeInsets.all(12),
              itemCount: animals.length,
              gridDelegate:
                  const SliverGridDelegateWithFixedCrossAxisCount(
                crossAxisCount: 2,
                crossAxisSpacing: 12,
                mainAxisSpacing: 12,
                childAspectRatio: 0.85,
              ),
              itemBuilder: (context, index) {
                final animal = animals[index];

                return GestureDetector(
                  onTap: () {
                    Navigator.push(
                      context,
                      MaterialPageRoute(
                        builder: (context) =>
                            AnimalDetailsPage(animal: animal),
                      ),
                    );
                  },
                  child: Card(
                    elevation: 4,
                    clipBehavior: Clip.antiAlias,
                    shape: RoundedRectangleBorder(
                      borderRadius: BorderRadius.circular(15),
                    ),
                    child: Column(
                      children: [
                        Expanded(
                          child: Image.network(
                            animal.image,
                            width: double.infinity,
                            fit: BoxFit.cover,
                            errorBuilder: (context, error, stack) {
                              return const Center(
                                child: Icon(
                                  Icons.pets,
                                  size: 60,
                                  color: Colors.teal,
                                ),
                              );
                            },
                          ),
                        ),
                        Padding(
                          padding: const EdgeInsets.all(12),
                          child: Text(
                            animal.name,
                            style: const TextStyle(
                              fontSize: 18,
                              fontWeight: FontWeight.bold,
                            ),
                          ),
                        ),
                      ],
                    ),
                  ),
                );
              },
            ),
          ),
        ],
      ),
    );
  }
}

// ANIMAL DETAILS PAGE
class AnimalDetailsPage extends StatelessWidget {
  final Animal animal;

  const AnimalDetailsPage({
    super.key,
    required this.animal,
  });

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text(animal.name),
        backgroundColor: Colors.teal,
        foregroundColor: Colors.white,
      ),
      body: SingleChildScrollView(
        child: Column(
          crossAxisAlignment: CrossAxisAlignment.start,
          children: [
            Image.network(
              animal.image,
              height: 250,
              width: double.infinity,
              fit: BoxFit.cover,
              errorBuilder: (context, error, stack) {
                return const SizedBox(
                  height: 250,
                  child: Center(
                    child: Icon(Icons.pets, size: 80),
                  ),
                );
              },
            ),
            Padding(
              padding: const EdgeInsets.all(20),
              child: Column(
                crossAxisAlignment: CrossAxisAlignment.start,
                children: [
                  Text(
                    animal.name,
                    style: const TextStyle(
                      fontSize: 30,
                      fontWeight: FontWeight.bold,
                      color: Colors.teal,
                    ),
                  ),
                  const SizedBox(height: 15),
                  Text(
                    animal.description,
                    style: const TextStyle(fontSize: 17),
                  ),
                  const SizedBox(height: 25),
                  detailItem(Icons.restaurant, 'Food', animal.food),
                  detailItem(Icons.home, 'Habitat', animal.habitat),
                  detailItem(Icons.favorite, 'Lifespan', animal.lifespan),
                  const SizedBox(height: 20),
                  const Text(
                    'Did You Know? 💡',
                    style: TextStyle(
                      fontSize: 22,
                      fontWeight: FontWeight.bold,
                    ),
                  ),
                  const SizedBox(height: 10),
                  Text(
                    animal.fact,
                    style: const TextStyle(fontSize: 17),
                  ),
                ],
              ),
            ),
          ],
        ),
      ),
    );
  }

  Widget detailItem(IconData icon, String title, String value) {
    return Padding(
      padding: const EdgeInsets.only(bottom: 18),
      child: Row(
        crossAxisAlignment: CrossAxisAlignment.start,
        children: [
          Icon(icon, color: Colors.teal, size: 27),
          const SizedBox(width: 12),
          Expanded(
            child: Column(
              crossAxisAlignment: CrossAxisAlignment.start,
              children: [
                Text(
                  title,
                  style: const TextStyle(
                    fontSize: 18,
                    fontWeight: FontWeight.bold,
                  ),
                ),
                const SizedBox(height: 4),
                Text(value, style: const TextStyle(fontSize: 16)),
              ],
            ),
          ),
        ],
      ),
    );
  }
}
# -Pets-Information-
About the pets 
