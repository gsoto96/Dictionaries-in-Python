# Dictionaries-in-Python
{
  "metadata": {
    "language_info": {
      "codemirror_mode": {
        "name": "python",
        "version": 3
      },
      "file_extension": ".py",
      "mimetype": "text/x-python",
      "name": "python",
      "nbconvert_exporter": "python",
      "pygments_lexer": "ipython3",
      "version": "3.8"
    },
    "kernelspec": {
      "name": "python",
      "display_name": "Pyolite",
      "language": "python"
    }
  },
  "nbformat_minor": 4,
  "nbformat": 4,
  "cells": [
    {
      "cell_type": "markdown",
      "source": "Dictionaries in Python\nEstimated time needed: 25 minutes\n\nObjectives\nAfter completing this lab you will be able to:\n\nWork with and perform operations on dictionaries in Python",
      "metadata": {}
    },
    {
      "cell_type": "code",
      "source": "# Create the dictionary\n\nDict = {\"key1\": 1, \"key2\": \"2\", \"key3\": [3, 3, 3], \"key4\": (4, 4, 4), ('key5'): 5, (0, 1): 6}\nDict",
      "metadata": {
        "trusted": true
      },
      "execution_count": 285,
      "outputs": [
        {
          "execution_count": 285,
          "output_type": "execute_result",
          "data": {
            "text/plain": "{'key1': 1,\n 'key2': '2',\n 'key3': [3, 3, 3],\n 'key4': (4, 4, 4),\n 'key5': 5,\n (0, 1): 6}"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# Access to the value by the key\n\nDict[\"key1\"]",
      "metadata": {
        "trusted": true
      },
      "execution_count": 286,
      "outputs": [
        {
          "execution_count": 286,
          "output_type": "execute_result",
          "data": {
            "text/plain": "1"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# Access to the value by the key\n\nDict[(0, 1)]",
      "metadata": {
        "trusted": true
      },
      "execution_count": 287,
      "outputs": [
        {
          "execution_count": 287,
          "output_type": "execute_result",
          "data": {
            "text/plain": "6"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# Create a sample dictionary\n\nrelease_year_dict = {\"Thriller\": \"1982\", \"Back in Black\": \"1980\", \\\n                    \"The Dark Side of the Moon\": \"1973\", \"The Bodyguard\": \"1992\", \\\n                    \"Bat Out of Hell\": \"1977\", \"Their Greatest Hits (1971-1975)\": \"1976\", \\\n                    \"Saturday Night Fever\": \"1977\", \"Rumours\": \"1977\"}\nrelease_year_dict",
      "metadata": {
        "trusted": true
      },
      "execution_count": 288,
      "outputs": [
        {
          "execution_count": 288,
          "output_type": "execute_result",
          "data": {
            "text/plain": "{'Thriller': '1982',\n 'Back in Black': '1980',\n 'The Dark Side of the Moon': '1973',\n 'The Bodyguard': '1992',\n 'Bat Out of Hell': '1977',\n 'Their Greatest Hits (1971-1975)': '1976',\n 'Saturday Night Fever': '1977',\n 'Rumours': '1977'}"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# Get value by keys\n\nrelease_year_dict['Thriller'] ",
      "metadata": {
        "trusted": true
      },
      "execution_count": 289,
      "outputs": [
        {
          "execution_count": 289,
          "output_type": "execute_result",
          "data": {
            "text/plain": "'1982'"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# Get value by key\n\nrelease_year_dict['The Bodyguard'] ",
      "metadata": {
        "trusted": true
      },
      "execution_count": 290,
      "outputs": [
        {
          "execution_count": 290,
          "output_type": "execute_result",
          "data": {
            "text/plain": "'1992'"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# Get all the keys in dictionary\n\nrelease_year_dict.keys() ",
      "metadata": {
        "trusted": true
      },
      "execution_count": 291,
      "outputs": [
        {
          "execution_count": 291,
          "output_type": "execute_result",
          "data": {
            "text/plain": "dict_keys(['Thriller', 'Back in Black', 'The Dark Side of the Moon', 'The Bodyguard', 'Bat Out of Hell', 'Their Greatest Hits (1971-1975)', 'Saturday Night Fever', 'Rumours'])"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# Get all the values in dictionary\n\nrelease_year_dict.values() ",
      "metadata": {
        "trusted": true
      },
      "execution_count": 292,
      "outputs": [
        {
          "execution_count": 292,
          "output_type": "execute_result",
          "data": {
            "text/plain": "dict_values(['1982', '1980', '1973', '1992', '1977', '1976', '1977', '1977'])"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# Append value with key into dictionary\n\nrelease_year_dict['Graduation'] = '2007'\nrelease_year_dict",
      "metadata": {
        "trusted": true
      },
      "execution_count": 293,
      "outputs": [
        {
          "execution_count": 293,
          "output_type": "execute_result",
          "data": {
            "text/plain": "{'Thriller': '1982',\n 'Back in Black': '1980',\n 'The Dark Side of the Moon': '1973',\n 'The Bodyguard': '1992',\n 'Bat Out of Hell': '1977',\n 'Their Greatest Hits (1971-1975)': '1976',\n 'Saturday Night Fever': '1977',\n 'Rumours': '1977',\n 'Graduation': '2007'}"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# Delete entries by key\n\ndel(release_year_dict['Thriller'])\ndel(release_year_dict['Graduation'])\nrelease_year_dict",
      "metadata": {
        "trusted": true
      },
      "execution_count": 294,
      "outputs": [
        {
          "execution_count": 294,
          "output_type": "execute_result",
          "data": {
            "text/plain": "{'Back in Black': '1980',\n 'The Dark Side of the Moon': '1973',\n 'The Bodyguard': '1992',\n 'Bat Out of Hell': '1977',\n 'Their Greatest Hits (1971-1975)': '1976',\n 'Saturday Night Fever': '1977',\n 'Rumours': '1977'}"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# Verify the key is in the dictionary\n\n'The Bodyguard' in release_year_dict",
      "metadata": {
        "trusted": true
      },
      "execution_count": 295,
      "outputs": [
        {
          "execution_count": 295,
          "output_type": "execute_result",
          "data": {
            "text/plain": "True"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# Question sample dictionary\n\nsoundtrack_dic = {\"The Bodyguard\":\"1992\", \"Saturday Night Fever\":\"1977\"}\nsoundtrack_dic ",
      "metadata": {
        "trusted": true
      },
      "execution_count": 300,
      "outputs": [
        {
          "execution_count": 300,
          "output_type": "execute_result",
          "data": {
            "text/plain": "{'The Bodyguard': '1992', 'Saturday Night Fever': '1977'}"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# a) In the dictionary soundtrack_dic what are the keys\nsoundtrack_dic.keys() ",
      "metadata": {
        "trusted": true
      },
      "execution_count": 301,
      "outputs": [
        {
          "execution_count": 301,
          "output_type": "execute_result",
          "data": {
            "text/plain": "dict_keys(['The Bodyguard', 'Saturday Night Fever'])"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# b) In the dictionary soundtrack_dic what are the values ?\nsoundtrack_dic.values() ",
      "metadata": {
        "trusted": true
      },
      "execution_count": 302,
      "outputs": [
        {
          "execution_count": 302,
          "output_type": "execute_result",
          "data": {
            "text/plain": "dict_values(['1992', '1977'])"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# The Albums Back in Black, The Bodyguard and Thriller have the following music recording sales in millions 50, 50 and 65 respectively:\n\n# a) Create a dictionary album_sales_dict where the keys are the album name and the sales in millions are the values.\n\nalbum_sales_dict = {\"Back in Black\": 50, \"Bodyguard\": 50, \"Thriller\": 65}\nalbum_sales_dict",
      "metadata": {
        "trusted": true
      },
      "execution_count": 313,
      "outputs": [
        {
          "execution_count": 313,
          "output_type": "execute_result",
          "data": {
            "text/plain": "{'Back in Black': 50, 'Bodyguard': 50, 'Thriller': 65}"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# b) Use the dictionary to find the total sales of Thriller:\nalbum_sales_dict[\"Thriller\"] \n",
      "metadata": {
        "trusted": true
      },
      "execution_count": 314,
      "outputs": [
        {
          "execution_count": 314,
          "output_type": "execute_result",
          "data": {
            "text/plain": "65"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# c) Find the names of the albums from the dictionary using the method keys():\nalbum_sales_dict.values()",
      "metadata": {
        "trusted": true
      },
      "execution_count": 317,
      "outputs": [
        {
          "execution_count": 317,
          "output_type": "execute_result",
          "data": {
            "text/plain": "dict_values([50, 50, 65])"
          },
          "metadata": {}
        }
      ]
    },
    {
      "cell_type": "code",
      "source": "# d) Find the values of the recording sales from the dictionary using the method values:",
      "metadata": {},
      "execution_count": null,
      "outputs": []
    }
  ]
}
